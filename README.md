## Jenkins Installation on CentOS 7


Jenkins is an open source, Java-based automation server that offers an easy way to set up a continuous integration and continuous delivery (CI/CD) pipeline.


This playbook installs Jenkins on CentOS 7.

1. Jenkins is a Java application, so the first step is to install Java. Run the following command to install the OpenJDK 8 package:

2. The next step is to add repository to your system

3. Then import gpg key for the repository

4. Install Jenkins

5. Start Jenkins and enable Jenkins

6. Get the Administrator password to unlock Jenkins

7. Print the password as message

8. Adjust the firewall, if necessary


* Run the playbook with the following command:

ansible-playbook jenkins-centos7.yml | sed 's/\\n/\n/g'

If the installation was successfull, at the end of run, you should see:

    -Jenkins login:
    -Administrator password:

    * NOTE: If you see "\n" at the end of password, don't copy the "\n". 
