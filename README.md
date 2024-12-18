<h1 align="center">Job Finder Website by @zeynepcol</h1> 

https://github.com/user-attachments/assets/b5f2f0ef-32b6-477b-a79a-7271596789c4

<br></br>
 <h3 align="center">JOB FINDER WEBSITE</h3>

**Job Finder** is a **web** application designed to connect job seekers with available job opportunities. The platform provides features for job listings, filtering, application management, and an admin panel to manage job postings and user interactions.

---

## Features

- **Job Seekers:**
  - Browse job postings with detailed information such as job title, description, requirements, and location.
  - Filter job listings by criteria including location, job type (full-time, part-time, remote), and category.
  - Apply for jobs directly through an intuitive interface.
  - Track application statuses and receive notifications for updates.

- **Admin Panel:**
  - Add, edit, and delete job postings with rich text editing support.
  - View and manage job applications, including exporting data for reporting.
  - Manage user accounts (activate/deactivate, view application history).
  - Publish company news and updates to inform job seekers.

- **Authentication and Authorization:**
  - Role-based access control to ensure only admins access administrative functionalities.

- **Scalability:**
  - Modular architecture to allow easy addition of new features.
  - Optimized database queries using LINQ for high performance.

---

## Technologies Used

- **Frontend:**
  - HTML, CSS
  - JavaScript
  

- **Backend:**
  - ASP.NET
  - C#
  - Entity Framework Core

- **Database:**
  - MSSQL Server

---

## Installation and Setup

Follow these steps to set up the project on your local machine:

### Prerequisites

- .NET Framework installed (version 4.7.2 or higher) or .NET Core SDK for cross-platform compatibility.
- Visual Studio (i used 2022 version) with ASP.NET and web development workloads.
- MSSQL Server installed and running.
- Git for version control.

### Steps

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/zeynepcol/Job-Finder.git
   cd Job-Finder
   ```

2. **Open the Project in Visual Studio:**
   - Open the `Job-Finder.sln` file in Visual Studio.

3. **Restore NuGet Packages:**
   - In Visual Studio, go to the **Tools** menu, then select **NuGet Package Manager** > **Manage NuGet Packages for Solution**.
   - Ensure all required packages are restored automatically.

4. **Set Up the Database:**
   - Open the `appsettings.json` file in the `JobFinder.Web` project.
   - Update the `ConnectionStrings:DefaultConnection` section with your MSSQL Server credentials:
     ```json
     {
       "ConnectionStrings": {
         "DefaultConnection": "Server=YOUR_SERVER;Database=JobFinderDB;Trusted_Connection=True;"
       }
     }
     ```
   - Open the **Package Manager Console** in Visual Studio and run the following commands to create and seed the database:
     ```bash
     Add-Migration InitialCreate
     Update-Database
     ```

5. **Configure the Startup Project:**
   - Right-click on the `JobFinder.Web` project in the Solution Explorer and select **Set as Startup Project**.

6. **Run the Application:**
   - Press `F5` or click the **Start** button in Visual Studio to launch the application.
   - The application will open in your default browser at `http://localhost:5000` or a similar URL.



## Usage

### For Job Seekers
- Register an account and log in to start exploring job opportunities.
- Use filters to refine job search results.
- Apply for jobs and track your application history from the dashboard.

### For Admins
- Log in with an admin account to access the admin panel.
- Add, edit, or remove job listings.
- View and manage job applications, including exporting application data.
- Manage registered users and post company updates.

---


## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch (`feature/your-feature`).
3. Commit your changes with detailed messages.
4. Push to the branch and create a pull request.

---

## Contact

For any questions or feedback, please contact:
- **Zeynep ÇÖL**  
  [GitHub Profile](https://github.com/zeynepcol)
