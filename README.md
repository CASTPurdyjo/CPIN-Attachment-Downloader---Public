# The CPIN Attachment Downloader

Welcome to the homepage for the CPIN Attachment Downloader.

Here you will find any updates on development as well as the roadmap of features that are planned for this project. Any features that have been implemented in the latest version will be crossed off in the roadmap.

You can find the latest version of the downloader here! (Will be inserting a link once a version is available teehee)

*This project developed on my own personal time and any issues that arise will be worked on during after hours and on weekends. If any immediate assistance is required, please email me and let me know the situation and while I am unable to work on this project during work hours, I will prioritize your request when I am relieved* 

## Roadmap

There are a number of things that need to be developed and improved upon from the previous experiment.
They will be subdivided into the following categories:

- Back End *(Important behind the scenes stuff that you don't necessarily see)*
- Front End *(User interface, making sure this thing is not only pretty but intuitive and user friendly)*
- User Functionality *(The meat and potatoes. Pulling files from different cases with different roles etc)*
- Lessons Learned *(Issues that have been outstanding or have bothered me about the previous version that I'd like to fix)*

### Back End - 

- Google Analytics API
    - Implement the same functionality that exists in the current version (*though cleaned up*) so that I can track usage and build a case for this to be implemented into CPIN
- Bitbucket Issues API Integration - 75%
    - For automatic issue creation
    - This is so if the program crashes or runs into an issue I can have the program automatically add an issue to the project so that I know about it immediately and can get the details on what occurred
- Concurrent Case Downloading
    - It sure would be nice to throw a bunch of case #s into this and it just automatically do them all (*even potentially at the same time!*)
- ~~Program Log - 100%~~
    - ~~Have a detailed output of what the program did at every step so if any issues pop up we can reference the log to see what happened~~
- Automatic Updating
    - This way everyone can update when ready and I don't need to chase after people anymore!

### Front End

- Develop an interface that supports multiple items in CPIN that can hold attachments (*participant, case, provider*) without feeling clunky
- Add tool bar items that can bring up this wiki, check for updates, see logs, and report bugs from inside the program
- Include more appropriate icons and feedback to notify a user of any issues or the current status of the program

### User Functionality

- Download attachments within specific date range (between 2 dates, before/ after date)
- Ability to exclude/include attachments based on Document type.
- Implement case types for different roles so users with different levels of access can use this program
    - Protection Worker Access
        - Person Record
        - Provider Record
        - Historical Case Record
        - Screening Case
        - Investigation Case
        - Ongoing Case
        - Child In Care Case
        - Adoption Case
        - Kinship Service Case
        - Voluntary Youth Service Agreement Case
        - Continued Care & Support for Youth Case
        - Renewed Youth Supports Case
        - Other Child Welfare Case
    - Supervisor Access
        - Person Record
        - Provider Record
        - Historical Case Record
        - Screening Case
        - Investigation Case
        - Ongoing Case
        - Child In Care Case
        - Adoption Case
        - Kinship Service Case
        - Voluntary Youth Service Agreement Case
        - Continued Care & Support for Youth Case
        - Renewed Youth Supports Case
        - Other Child Welfare Case
    - Local Administrator Access
        - Person Record
        - Provider Record
        - Historical Case Record
        - Screening Case
        - Investigation Case
        - Ongoing Case
        - Child In Care Case
        - Adoption Case
        - Kinship Service Case
        - Voluntary Youth Service Agreement Case
        - Continued Care & Support for Youth Case
        - Renewed Youth Supports Case
        - Other Child Welfare Case

### Lessons Learned
     
- Handle situation where there are no items to combine into a pdf. Apparently the program just crashes!
- Install the program in program files/where user wants
    - Used a simple tool called "ClickOnce" which forces users to install the program into their own profile
- Prompt for password on every use
    - While I'm sure people enjoyed the simple run and go, for security reasons this really should be something that you input every time
- Exclude attachments from other agencies
    - Not sure if this is actually possible but I want to check that out
- Exclude any attachments that have been marked privileged 
- Handle scenario where attachments have super long names
    - Apparently there are some attachments in the system that have a name so long that Windows throws an error at me when trying to save it somewhere
