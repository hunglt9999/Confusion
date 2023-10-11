%%{init: {'theme': 'neutral'}}%%
swimlane "Job Seeker" as JS
swimlane "Employer" as ER
swimlane "System" as SYS

JS->SYS: Create user account
SYS->JS: Confirm account creation
JS->SYS: Update profile information 
SYS->JS: Profile updated
JS->SYS: Search and view job listings
SYS->JS: Display search results
JS->SYS: Apply to job posting
SYS->ER: Forward job application
ER->SYS: Review application
ER->JS: Schedule interview
JS->ER: Attend interview
ER->SYS: Record interview result
SYS->JS: Notify interview result
JS->ER: Accept/Reject job offer
ER->SYS: Record offer result  
SYS->JS: Confirm job offer result