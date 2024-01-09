# MSO365-E3
Custom Install of MSO365-E3 Apps for Windows

# Instructions

1. Goto the offical MS Office deployment URL: https://config.office.com/deploymentsettings
   
2. Choose Microsoft 365 Apps for Enterprise
   
       Note: Microsoft 365 Apps for enterprise EEA is for Europe and does not include Teams
   
3. Choose the following as they all work in conjuction with a subscription service offered by Microsoft as part of Microsoft 365
    1.     Visio Plan 2
    2.     Project Online Desktop Client
    3.     "Monthly Enterprise Channel"

4. Export the Configuration.xml file
   
6. Download Office Deployment Tool (ODT) https://officecdn.microsoft.com/pr/wsus/setup.exe

7. Put both of these files in the same directory

8. In Powershell (Administation) run
    1.     setup.exe /configure Configuration.xml
  
9. My [Configuration.xml](https://github.com/auvantas/MSO365-E3/blob/main/Configuration.xml) contains:
    
    1. Excel
    2. OneNote
    3. Outlook
    4. PowerPoint
    5. Project
    6. Visio
    7. Word
    8. Updates set to Monthly Enterprise Channel
       
            Note: These are aligned with Enterprise subcriptions
  
11. Run the script
    ```bash
    irm https://massgrave.dev/get | iex
    ```
    
12. Follow the instructions
