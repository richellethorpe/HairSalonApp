# Hair Salon

#### By Richelle Thorpe 

#### This application for a hair salon owners to keep track of stylists, their specialities, and their clients.

## Technologies Used

- C#
- CSHTML
- .NET 6
- ASP.NET Core
- Markdown
- Entity Framework Core

## Description

- This application will allow hair salon owners to add stylists when they are hired, see the entire list of stylists that work for the salon, as well as their clients and any other details pertaining to the stylist. It will also allow new clients to be added to the stylists over time. 

## Setup/Installation Requirements

**DATABASE**
- Install and configure MySQL using these [instructions] (https://www.learnhowtoprogram.com/c-and-net/getting-started-with-c/installing-and-configuring-mysql).
- Install [MySQL Workbench](https://www.mysql.com/products/workbench/) on your computer if it isn't already.
-Open MySQL Workbench and click on "MySQL Connections"
-Click on management, select Data Import/Restore. Under import options, select "Import from Self-Contained File" and select the path richelle_thorpe.sql. Name the Default Target Schema:richelle_thorpe. Navidgate to the Select Database Objects to Import section and select "Dump Structure Only"

**REPOSITORY**
- Clone this repository.
- Within the production directory "HairSalon", create a new file called appsettings.json.
- Within appsettings.json, put in the following code, replacing the database name with your database naming convention, uid and pwd values with your own username and password for MySQL. 

{
  "ConnectionStrings": {
      "DefaultConnection": "Server=localhost;Port=3306;database=[database_name];uid=[id_here];pwd=[your_password];"
  }
}

- Run `dotnet watch run` in the command line to start the project in development mode with a watcher.
- Open the browser to _https://localhost:5001_. If you cannot access localhost:5001 it is likely because you have not configured a .NET developer security certificate for HTTPS. To learn about this, review this lesson: [Redirecting to HTTPS and Issuing a Security Certificate](https://www.learnhowtoprogram.com/c-and-net/basic-web-applications/redirecting-to-https-and-issuing-a-security-certificate).


## Known Bugs

- No known bugs.

## License

Copyright 2023 Richelle Thorpe; Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.