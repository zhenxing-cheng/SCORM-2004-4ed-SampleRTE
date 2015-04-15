# SCORM-2004-4ed-SampleRTE

1. sudo apt-get install openjdk-6-jdk
2. download apache-ant-1.7.1-bin.tar.bz2
3. download and install tomcat per these instructions - https://www.mulesoft.com/tcat/tomcat-60 - then move to apache-tomcat folder
3. sudo nano /etc/environment (add JAVA_HOME="/path/to/java-1.6.0-openjdk-amd64", ANT_HOME="path/to/ant",
SCORM4ED_SRTE111_HOME="path/to/created/dir/SCORM_2004_4th_Ed_Sample_RTE_V1.1.1",
SCORM4ED_TS111_HOME="path/to/created/dir/SCORM_2004_4th_Ed_Sample_RTE_V1.1.1",
CATALINA_HOME="path/to/created/dir/SCORM_2004_4th_Ed_Sample_RTE_V1.1.1/Sample_RTE/apache-tomcat")
4. add ${JAVA_HOME}/bin:${ANT_HOME}/bin to the end of PATH in /etc/environment
5. anytime a terminal is opened, be sure to run `. /etc/environment`
6. create/download api, bin, css, RTE_Readme folders and place in Sample_RTE folder (simulates running the installer)
7. make sure jdom, commons-fileupload, commons-io are all in adl/web-inf/lib
8. make sure all of the previous step jars plus adlvalidation, cmidatamodel, lmsclient, squencer, sqlite, and util are in apache-tomcat/lib
9. set rteFilesDir in build.properies to your home directory (/home/username)


