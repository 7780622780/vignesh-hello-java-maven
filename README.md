# Hello Java Maven – Jenkins Build

This project is a simple Java application (`HelloWorld.java`) built with **Maven** and automated using **Jenkins**.  
It demonstrates setting up a Jenkins Freestyle job, integrating GitHub as the source repository, and running `mvn clean package` to compile and package the code.  

---

Project Details
- **Technology Stack:** Java, Maven, Jenkins  
- **Build Tool:** Apache Maven (`clean package`)  
- **CI Server:** Jenkins (Freestyle Project)  
- **Repository:** GitHub  

---

Project Structure
hello-java-maven/
├── pom.xml
└── src/
└── main/
└── java/
└── HelloWorld.java

---

## ⚙️ Steps Performed
1. Created a simple `HelloWorld.java` file and `pom.xml`.  
2. Installed Jenkins in Docker and unlocked it using the initial admin password.  
3. Installed **suggested plugins** (Git, Maven, etc.).  
4. Configured **Global Tool Configuration** → added Maven.  
5. Created a **Freestyle project** in Jenkins.  
6. Linked GitHub repo under **Source Code Management**.  
7. Added **Build Step → Invoke top-level Maven targets** with `clean package`.  
8. Triggered the build → Maven compiled the project and packaged the JAR.  
9. Verified the build with **BUILD SUCCESS** in Console Output.  

---

## 📸 Jenkins Build Proof
Screenshot of Jenkins Console Output showing successful build:

Build Success.png

---

## ▶️ How to Run Locally
1. Clone the repo:
   ```bash
   git clone https://github.com/7780622780/vignesh-hello-java-maven.git
   cd vignesh-hello-java-maven
