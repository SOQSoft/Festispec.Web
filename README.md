
# Festispec.Web

## Installation

 **1.**  Clone de repository 
 
 **2.**  Open Command promp 
 
 **3.**  `cd` naar de map met het project 
 
 **4.** Voer de volgende commando's uit
```cmd
#Restore npm packages
dotnet restore

# Restore database
dotnet ef database update

# Run project 
dotnet run
```

## Development

Om de webapplicatie te draaien via cmd voer de volgende commando's uit
```cmd
#Restore npm packages
dotnet restore

# Restore database
dotnet ef database update

# Run project 
dotnet run
```


## Testing

### Tests draaien doormiddel van command line 
Het is mogelijk om via bash of cmd te draaien hiervoor moet je de volgende commando's invoeren: 
``` 
#Restore npm packages
dotnet restore

# Restore database
dotnet ef database update

# Run tests
dotnet test
```
### Tests draaien door middel van Visual studio
1.  Open  **Test Explorer**.
    
    ![On the Test menu, open Test Explorer](https://docs.microsoft.com/en-us/visualstudio/test/media/rununittest1.png?view=vs-2017)
    
2.  Run unit tests.
    
    ![Run unit tests in Test Explorer](https://docs.microsoft.com/en-us/visualstudio/test/media/rununittest2.png?view=vs-2017)
    
    Je kan in de de valende en werkende tests zien in  **Test Explorer**.
    
    ![Review unit test results in Test Explorer](https://docs.microsoft.com/en-us/visualstudio/test/media/rununittest3.png?view=vs-2017)


## Deployment
### Deployment method
Deployments gaan automatish doormiddel van intergratie van azure devops, zodra er iets naar de develop branch wordt gepushed wordt deze automatish op de test server gedeployed. 
Wil je het deployen naar de master server push dan de code van develop naar  ``Release`` aan in github, 


1.  Open Github en navigeer naar de repository.
    
2.  Under your repository name, click **Releases**.
  <img src="https://help.github.com/assets/images/help/releases/release-link.png" width="818"/>    
3.  klik op **Draft a new release**.
  <img src="https://help.github.com/assets/images/help/releases/draft_release_button.png" width="371"/>

4.  ![Releases tagged version](https://github.com/SOQSoft/Technisch-Ontwerp/wiki/Versiebeheer =360x49) Schrijf het versie nummer neer van welke versie het is gebruik hierbij de benaming van het het  [versie beheer](https://git-scm.com/book/en/Git-Basics-Tagging) van het technish ontwerp.

5. Selecteer de master branch  pak geen andere branch anders kunnen testen fout gaan.
  <img src="https://help.github.com/assets/images/help/releases/releases_tag_branch.png" width="356"/>
  
6. Schijf een titel en een beschrijving met wat er in deze release zit.  
  <img src="https://help.github.com/assets/images/help/releases/releases_description.png" width="401"/>
7.  Als je hem wilt releasen maar niet wilt deployen naar productie zet hem dan naar **This is a pre-release** dan zou hij door de  tweede test server in gebruik worde genomen. 
  <img src="https://help.github.com/assets/images/help/releases/prerelease_checkbox.png" width="400"/>
  
8.  Als je klaar bent om het te deployen klik dan op **Publish release**, wil je nog even wachten klik dan op **safedraft**
  <img src="https://help.github.com/assets/images/help/releases/release_buttons.png" width="200"/>

9. Kijk op [Azure devops](https://dev.azure.com/Festispec/FestispecApp/_workitems/assignedtome/) om te zien wat de status van de deployment is.
