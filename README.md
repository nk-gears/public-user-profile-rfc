Initial Proposal to Standardize Public Profile using a simple .yml file

### Background 

Traditional way of Sharing Profiles in Phones uses VCARD File
[(VCard, JCARD) - Wiki ](https://en.wikipedia.org/wiki/VCard#jCard)

### Summary

In this RFC, I am proposing a standardized way to create public profiles and share them easily to other applications. This standardized proposal will not includes and personal details like Phone Number, Address etc. This focusses mostly on the user digital presence and the corresponding links to their works, blogs and any other public account which they want to share with anyone.

### Challenges
- With the increasing number of applications used by users, each of these application is using a Custom Registration form, OAuth based/SSO based Integration to collect the profile information. Once registered, the profile details are not updated on regular basis. Either some of the information are obsolette (assume the user blog site is moved to a different site)
- Even the Author doesn't have a common way to manage and update their profiles and keep the version history.


### How if everyone has a common profile file :

- Asssume a user ABC, maintains his profile using a source control version like GitHub.com. They can create multiple profiles and share wherever needed with just a Url/file.

(e.g) 
http://github.com/<ABC>/my-profiles/default-profile.yml
http://github.com/<ABC>/my-profiles/work-profile.yml
  

Applications who want to get the user profile information, they can simply read the yaml file and update them on regular intervals.

Sample default-profile.yml

```
website: gyanmoti.in
country: india
name: Nirmal
profile_image_url: "https://media.licdn.com/dms/image/C4D03AQFgMmks5SVa_w/profile-displayphoto-shrink_200_200/0?e=1566432000&v=beta&t=XehIjAJiGztgNbN42I5fY6RWvY8dpeN4J_czWn0IRY0"
social_accounts: 
  - facebook: NA
  - twitter: nirmal_kumar
  - youtube: NA
  - linked_in: nirmalweb
creations:
  - courses: http://usercourses.com
  - publications: http://userpublications
  - podcasts: http://userpodcasts

```

Hereby requesting your comments for this public profile and make the web a better place to share and manage one's own profile.


