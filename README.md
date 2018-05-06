# JavaServer Pages (JSP) Hello World Sample

- Create new Dynamic Web Project in Spring Tool Suite IDE
- Create helloWorld.jsp file and run the project in Tomcat server

# Prerequisites

- Download and install JDK 9 in `C:\Program Files\Java\jdk-9.0.4` folder and add this path in `JAVA_HOME` and `PATH` environment variables
- Download and install `Apache Tomcat 9.0.6` in `C:\Dev\tools\apache-tomcat-9.0.6` folder

# Steps

- `File > New > Dynamic Web Project`
- Write `jsp-helloworld` for Project Name
- Select `Apache Tomcat v9.0` as `Target Runtime`
- Click `Modify` button for configuration and select `Dynamic Web Module 3.1` and `Java 9` facets
- Keep default settings as you navigate using `Next` button
- In the end select `Generate web.xml deployment descriptor`
- Click `Finish`
- Create `pages` folder under WebContent
- Right click `pages` folder, then `New > Other`
- Select JSP File and name it helloWorld.jsp and click Finish
- Change `<title>Insert title here</title>` to `<title>JSP Hello World Sample</title>`
- Inside body add `<%= "Hello World" %>`
- Right click project: `Build Path > Configure Build Path… > Deployment Assembly > Add… > Folder` then select `WebContent\pages` folder
- Right click project: `Run > Run As > Run on Server` and select `Tomcat v9.0 Server` and add server runtime environment using folder `C:\Dev\tools\apache-tomcat-9.0.6`
- After adding server, STS will start Tomcat server and open http://localhost:8080/jsp-helloworld/helloWorld.jsp with Hello World text
