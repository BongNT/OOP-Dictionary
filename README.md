# USER'S GUIDE

/**
 * @Author Anh Pham, Thanh Bong 
 * K64 CACLC3
 * UET VNU
 */

## STEP 1 : SET UP IN IDE
- Clone project from GitHub Repository URL : *https://github.com/anhpham197/DictionaryUET.git*
- Add a Maven Dependency to your project :
 + Add these lines in this link into file **pom.xml** : *https://pastebin.com/0gLA52JV*
 + Reload project.
- Setting **Environment Variables**:
 + Open System Properties dialog -> Advanced -> Environment variables
 + Create new **System variables** with *Variable* : **GOOGLE_APPLICATION_CREDENTIALS**
                                        *Value*    : path to **dictionary-uet-5a1633bd8e16.json** in package **lib**
                                                Eg : C:\Users\DELL\OneDrive\Máy tính\DictionaryUET\dictionary-uet-5a1633bd8e16.json
                                            Detail : *https://www.twilio.com/blog/2017/01/how-to-set-environment-variables.html*
                                            
## STEP 2 : SET UP DATABASE SYSTEM (MYSQL)
- Open package **lib** and add **mysql-connector-java-8.0.20.jar** into external libraries.
- After downloading MySQL Community Server, open file **lib\ConnectToDB.txt** to and replace with your **localhost, username, pass** in MySQL as example.
- Restore database: 
 + Open MySQL -> Server -> Data Import
 + Select **Import from Self-Contained file** and chose path to **DictionaryDB_backup.sql** in package **lib**
 + Create new *Target Schema* named **dictionarytest** 
 + Select **Start Import**
 
## STEP 3 : RUN PROJECT (Main.java)