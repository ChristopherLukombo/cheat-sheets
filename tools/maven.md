# Maven

Apache Maven is a software project management and comprehension tool. Based on the concept of a project object model (POM), Maven can manage a project's build, reporting and documentation from a central piece of information.

### Basics commands

| Maven Command | Comment |
| --- | --- |
| `mvn dependency:analyze` | Analyze dependencies |
| `mvn dependency:tree`   | Performs a dependency tree |
| `mvn -emp mypassword` | Encrypt the password |
| `mvn clean package -T 1C` | Performs a package with 1 thread per CPU |

### Encrypt password

####  Master password

Run the command : `mvn --encrypt-master-password objis`
 
create a blank file USER_HOME/.m2/**settings-security.xml** and report the result of the command:
 
That's it, the first step of securing your passwords is complete. The settings-security.xml file will be necessary for further operationss.

Maven will look for this file by default in USER_HOME/.m2 unless you tell it another location via ‘**relocation**’ tag.

#### Part 2: password

Let's assume that you are one of the few users with write access to the delivery deployment server. The authorized user has a 'deployment' password which you do not want to appear hard-coded in your settings.xml

Run the command : `mvn --encrypt-password deployment`

Update the settings.xml file by replacing the password with the command output.