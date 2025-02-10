Overview
This console application is designed to assist system administrators in efficiently retrieving and managing network-related information. It offers functionalities to search through Excel-based databases for specific keywords, ping individual IP addresses, and scan a range of IP addresses within a network. The application is developed in C# using Visual Studio 2022 and is currently under active development.

Features
Keyword Search: Searches through Excel files to find entries matching user-defined keywords, facilitating quick access to relevant data.
Ping Utility: Allows users to ping specified IP addresses to check their availability and response times.
Network Scan: Enables scanning of a specified range of IP addresses to identify active devices on the network.
Prerequisites
Operating System: Windows 10 or later
Development Environment: Visual Studio 2022
.NET Framework: .NET 6.0 or later
NuGet Packages:
ExcelDataReader
ExcelDataReader.DataSet
Installation
Clone the Repository:

bash
Copy
Edit
git clone https://github.com/yourusername/networking-tool.git
cd networking-tool
Open the Solution:

Launch Visual Studio 2022.
Open the NetworkingTool.sln solution file located in the cloned repository.
Restore NuGet Packages:

Navigate to the Solution Explorer.
Right-click on the solution and select "Restore NuGet Packages" to ensure all dependencies are installed.
Build the Solution:

Click on "Build" in the top menu.
Select "Build Solution" to compile the application.
Run the Application:

Press F5 or click on the "Start" button to run the application.
Usage
Upon running the application, you will be presented with a main menu offering the following options:

Search: Enter a keyword to search through the Excel databases. The application will display matching entries, allowing for quick data retrieval.
Ping: Input an IP address in the format xxx.xxx.xxx.xxx to ping. The application will continuously ping the specified address until the spacebar is pressed to stop.
Scan: Define a range of IP addresses to scan. The application will ping each address within the specified range and display active devices.
Exit: Close the application.
Note: Ensure that the Excel files you intend to search are formatted correctly and placed in the designated directory as specified in the application's configuration.

Excel File Format
The application expects Excel files to have a specific structure to function correctly. Below is an example of the expected format:

Device Name	IP Address	Location	Description
Device1	192.168.1.10	Office 1	Main office router
Device2	192.168.1.11	Office 2	Backup server
Device3	192.168.1.12	Data Center	Database server
Ensure that your Excel files follow this structure, with appropriate headers and data entries.

Deployment
For deployment purposes, the application, along with sample Excel files and necessary resources, is packaged in the following compressed files:

Application Package: 67_networking_tool.zip
Installation Package: !INSTALLATION!.zip
These packages contain the executable application, sample Excel files, and a Visual Studio 2022 solution file (.sln) for further development or customization.

Contribution
As this project is still under development, contributions are welcome. Feel free to fork the repository, make improvements, and submit pull requests. Please ensure that any contributions align with the project's coding standards and include appropriate documentation.

License
This project is licensed under the MIT License. See the LICENSE file for more details.
