# midway-hack

The idea is to create a GitHub App which organizations can install to see what team members are doing in the form of Feed using GitHub Webhooks.  
The feed will track following activities  
- Pull requests
- Issues
- Comments
- Commits 

The flow will be like this:
- Organization install app
- Go to somedomain/Org-Name
- All the activites are listed since the installation of app
- Filter events by team
- Filter events by Member

The App will have following components
- Vue Frontend
- NodeJs backend with SQLite Database

### backend 
- will utilize GitHub webhooks to get the subscribed events 
- It will store it on a SQLite database
- Provide APIs to return data to frontend

### Frontend
- A home page with installation instructions
- A dynamic feed page to render activities of an Org
