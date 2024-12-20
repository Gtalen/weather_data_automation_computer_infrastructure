



1. Workflow files Creation
- I started by creating a directory *.github* with a subdirectory *workflows*
- Subsequently, I created a file [weather_data.yml](https://github.com/Gtalen/computer_infrastructure/blob/main/.github/workflows/weather_data.yml) which contains the github actions workflow
- The github actions yml file was generated utilizing resources from github actions documentation, crontab gurus and chat gpt 4.0 detailed prompting.

2. Workflow Definition
    - The automated weather script  was set up to run by 10am daily
    - The script runs on the latest version of Ubuntu.
    - A git repository checkout step was included
    - workflow_dispatch was included to allow for manual trigger and testing of the git action
    - The change mode command step was included to ensure the script is execuatble
    - Execution of the [weather.sh](https://github.com/Gtalen/computer_infrastructure/blob/main/weather.sh) script
    - Commit and push changes back to my repository in the [weather directory](https://github.com/Gtalen/computer_infrastructure/tree/main/data/weather).

3. Script testing  using workflow dispatch in git actions
- The first execution of the git action returned a run error code due to permission restrictions.

4. Modifications and further testing
- The yml script was modified to include a gittoken. 
- Futhermore, a read and write permission settings adjustment was made on my github account to enable the script to commit and pull changes to my repository.
- Post-modification testing was successful.


