# Crowdfunding Back End
Caterina Lopez

## Planning:
### Concept/Name
A crowdfunding ecosystem designed to fund people, not just projects — where performers, individuals, and community groups receive financial support, encouragement, visibility, and collective belief to reach specific goals.

This isn’t charity.
It’s collective uplift.
Who It Serves
## Performers & Creators

Dancers, musicians, actors, spoken-word artists, athletes, cultural performers.

Goals may include:

Training and coaching

Travel to auditions, competitions, festivals

Equipment, costumes, studio time

Producing independent work

Support style:
Backers follow the journey, receive updates, behind-the-scenes access, performances, gratitude moments.
“Built by community. Powered by purpose.”
### Intended Audience/User Stories
Performaners and sporting groups.....

- As a user I can see a list of fundraisers on the homepage?
- As a user I can login to the website and see my profile
- As a user I can see an individual fundrasiers
- As a user I can see photos and/or videos of the fundrasier
- As a user I can comment on a fundraiser

### Front End Pages/Functionality
- Homepage
    - User Details
    - List Fundraisers
        - Individual Fundraiser

### API Spec

| URL | HTTP Method | Purpose | Request Body | Success Response Code | Authentication/Authorisation |
| --- | ----------- | ------- | ------------ | --------------------- | ---------------------------- |
| /fundraisers/ | GET |Return all fundraisers| N/A |200|N/A|
| /fundraisers/ | POST |Create a new fundraiser|Fundraiser object|201|Must be logged in|
| /fundraisers/:id | GET |Return fundraiser by ID|N/A|200|N/A|
| /fundraisers/:id | PUT |Update a fundraiser|Fundraiser object|200|Must be logged in and the owner|
| /api-token-auth/ | POST |to log in |username and password|200|anonymous|

### DB Schema
![]( {{ ./relative/path/to/your/schema/image.png }} )