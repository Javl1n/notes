# Guest - NonUser
## Welcome page
this page is for guests only, first page they go when they open the website or when they logout
**Contents:**
- Auth Button
	- Login
	- Register
- Coming **concerts**
	- 1 latest banner concert
	- grid concerts


## Show Concert
information of concert
**Contents**
- Info sa concert
- login to buy a ticket

# Organizer

## Dashboard
page where organizers can view their concert statistics, you can add more, wala ko kabalo unsa pay pwede mabutang diri

## Concerts

### Index
main page or index of concert management for organizer
**Contents**
- Book a Concert button - Create Concert
- Booked Concert List - each item redirects to their respective show page

### Create
where organizer can book concerts. it's a 2 page process:

#### Schedule Map
A calendar like interface to view what time can the organizer book for a concert.
- red if already booked
- green if you the organizer booked
- white / neutral if available
Pwede multiple days ang iselect
Organizers can click to white to book that time, then they proceed to filling up a form.

#### Concert Form
Where organizers can then fill up a form to book a time. please refer to the database for the inputs.
**Contents**
- Form (database)
	- DateTime Start & End - Dropdown
		- within sa iya giselect na days
	- pricing sa VIP ug General Admission
- Send Gcash QR
- I-select niya nag VIP nga seats
- Submit Button - Redirect to concerts/index page

### Show
information about a concert. concerts can't be cancelled.
**Contents**
- Information
	- QR Code
	- .aksdjaldjlaks
- Seating
- Update Button - redirects to concerts/update page

### Update
update information of a concert
**Contents**
- Save Button - redirects to concerts/show
- Form (database)
	- DateTime Start & End - Dropdown
		- within sa iya giselect na days
	- pricing sa VIP ug General Admission

# Concert Goer
## Home Page
Almost Similar to the welcome page
**Contents**
- Concert List - redirect to respective concert/show

## Concerts
### Index
Similar to home page, but more advanced, and consistent in design.
