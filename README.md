# Higher National Diploma in Science in Computing (Data Analytics)
## Atlantic Technological University (ATU) Galway
## Computer Infrastructure  Module (8645: 2024-2025)
## Author: Ebelechukwu Chidimma Igwagu

## Description
This repository showcases my work for the module computer infrastructure at ATU Galway. The objective of these tasks and the project is to demonstrate my proficiency in utilizing the Linux command line interface for various tasks such as data manipulation, scripting, workflow automation, and data migration.

## TASKS

This repository contains solutions to a series of seven tasks, along with corresponding script log files. The detailed explanations and solutions for each task can be found in the [weather.ipynb](https://github.com/Gtalen/computer_infrastructure/blob/main/weather.ipynb) notebook. 

### Task 1: Create Directory Structure
### Task 2: Timestamps
### Task 3: Formatting Timestamps
### Task 4: Create Timestamped Files
### Task 5: Download Today's Weather Data
### Task 6: Timestamp the Data
### Task 7: Bash Script
### Task 8: Report on Tasks
### Task 9: Weather Data Analysis
   

## PROJECT - Automating weather data download

In this project, I automated the [weather.sh](https://github.com/Gtalen/computer_infrastructure/blob/main/weather.sh) from task 7 above using the [weather_data.yml](https://github.com/Gtalen/computer_infrastructure/blob/main/.github/workflows/weather_data.yml) to run daily by 10 am using github actions. 

### Procedure

1. **Workflow File Creation**
   - I created a *.github* directory, followed by a *workflows* subdirectory to house the GitHub Actions workflow file.
   - The workflow file, [weather_data.yml](https://github.com/Gtalen/computer_infrastructure/blob/main/.github/workflows/  weather_data.yml), was used to define the automation process.
   - Resources for creating the workflow included GitHub Actions documentation, crontab tutorials, and detailed prompting from   ChatGPT-4.

2. **Workflow Definition**
   - The script is set to execute at 10 AM daily.
   - It runs on the latest Ubuntu version, ensuring compatibility with the script.
   - The workflow includes a git repository checkout step.
   - A workflow_dispatch trigger is added to allow for manual initiation and testing.
   - The chmod step ensures the script has executable permissions.
   - The script then executes the [weather.sh](https://github.com/Gtalen/computer_infrastructure/blob/main/weather.sh) file   updating the weather data.
   - Finally, the script commits and pushes changes to the repository in the [weather directory](https://github.com/Gtalen/  computer_infrastructure/tree/main/data/weather).

3. **Initial Testing and Error Handling**
   - The first execution encountered an error related to permission restrictions.

4. **Modifications and Further Testing**
   - The workflow YAML file was updated to include a GitHub token for authentication.
   - Permissions on my GitHub account were adjusted to allow the script to commit and push changes.
   - After these modifications, testing was successful, and the automation runs smoothly.
 

## Usage

To run the project and replicate the automation process:
- Clone the [repository](https://github.com/Gtalen/computer_infrastructure) using github codespaces by clicking on the green "code" button, select "Codespaces", and launch the environment.

- Launch the VScode setup environment in codespaces

- Use ctrl + shift + p and select Terminal: create new terminal in editor area to access the bash Shell in VS code

- Follow the steps outlined in the tasks and project to code along and see the automation in action.



## Technologies Used

  - GitHub Codespaces: Cloud-based development environment
  - Visual Studio Code: Code editor for project development
  - Bash: Scripting language used for task automation
  - GitHub Actions: For automating workflows and scheduled tasks
  - Python: Data processing and analysis
  - Pandas: Python library for data manipulation and analysis
  - Cron: Scheduling automated task

### Contributors

- Ebelechukwu Chidimma Igwagu: Project author

- Want to contribute?
  - This project is open to contributions. Feel free to submit issues or pull requests.

### License
This project is available under the MIT, GNU license.












