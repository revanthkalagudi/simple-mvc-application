# MVC App with User Management using Spring Boot

This repository provides a demonstration of the Model-View-Controller (MVC) architecture and the Spring Boot framework. MVC is a software design pattern that separates an application into three interconnected components: the model, the view, and the controller. The model represents the application's data and business logic, the view presents the data to the user, and the controller handles user input and updates the model and view accordingly.

Spring Boot, on the other hand, is a popular Java-based framework that simplifies the development of stand-alone, production-grade Spring applications. It provides a robust set of tools and conventions for building scalable and efficient applications. With its opinionated approach and auto-configuration capabilities, Spring Boot minimizes the effort required for setting up and configuring a Spring-based project.

This repository combines the power of MVC architecture and Spring Boot to create a sample application that showcases the principles and benefits of both. By exploring the code and the accompanying documentation, developers can gain a deeper understanding of how these technologies work together to build robust and maintainable applications.


## Requirements

1. IntelliJ IDEA (Ultimate Version) [Install](https://www.jetbrains.com/help/idea/installation-guide.html#toolbox)
2. MySQL Workbench [Install](https://dev.mysql.com/downloads/workbench/)




## Downloading and Running the MVC Application

Follow these step-by-step instructions to download and run the MVC application on IntelliJ IDEA and MySQL Workbench:

1. **Download the ZIP:** Go to the GitHub repository page and click on the "Code" button. From the dropdown menu, select "Download ZIP." This will download a compressed ZIP file containing the repository code to your local machine.

2. **Extract the ZIP File:** Once the ZIP file is downloaded, extract its contents to a desired location on your computer. You can use any extraction tool, such as WinRAR or 7-Zip, to extract the files.

3. **Import the Project:** Launch IntelliJ IDEA and select "Open" from the welcome screen. Navigate to the location where you cloned the repository and choose the project's root directory. Click "Open" to import the project.

4. **Configure the Database:** Before running the application, ensure that you have MySQL Server installed and running on your machine. **Open MySQL Workbench and create a new database with a suitable name for your application.** The database name that you use here should be the same as the database name that you provide in **applications.properties** file(Check Step 6).

5. **Update Application Configuration:** In the project, locate the application.properties file. Open it and update the following properties according to your MySQL configuration:


```php
spring.datasource.url=jdbc:mysql://localhost:3306/<database_name>
spring.datasource.username=<database_username>
spring.datasource.password=<database_password>
spring.jpa.hibernate.ddl-auto=update
spring.mvc.view.prefix=/WEB-INF/views/
spring.mvc.view.suffix=.jsp
```
Replace **<database_name>**, **<database_username>**, and **<database_password>** (remove the angular brackets(<>)) with your database's name, username, and password respectively.

6. **Build the Project:** Build the project in IntelliJ IDEA by selecting "Build" from the top menu and then choosing "Build Project." Ensure that the build process completes successfully without any errors.

7. **Run the Application:** Run the application by right-clicking on the main class file (typically named Application or Application.java) and selecting "Run" from the context menu. Alternatively, you can use the "Run" button located in the toolbar.

8. **Access the Application:** Once the application is running, open your web browser and navigate to http://localhost:8080. You should see the home page of the MVC application.

Congratulations! You have successfully downloaded and run the MVC application on IntelliJ IDEA and MySQL Workbench. Feel free to explore the code and make any necessary modifications to suit your requirements.


```
```
## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT][(https://choosealicense.com/licenses/mit/)](https://github.com/revanthkalagudi/simple-mvc-application/blob/main/LICENSE)
