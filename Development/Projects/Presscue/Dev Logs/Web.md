# Web To Do
## System Admin
### Authentication
- [x] Login
- [x] Logout
- [x] Profile
### Role
- [x] Store
- [x] Index
- [x] Show
- [ ] Add number of sectors of which there is an admin there
### Sectors
- [x] Store
- [x] Index
- [x] Show
- [x] Update
### Admin / User
- [x] Store
- [x] Index
- [x] Show
- [x] Add role id to users_table
### Patrollers
- [x] Index
## System
- [x] Setup sail for expose
- [x] Send kuya Jayson all end points
- [x] Setup local reverb to the sail repository
## Patroller
### Send Location
- [x] Send Every Interval
- [x] Update location if patroller travelled for more than 100 meters
- [x] send update to admin when location changes
- [x] Returns an Incident if patroller is dispatched
- [x] Returns no content if no dispatch
### Active Status Behavior
- [ ] icheck ang active status kung when ang last update sa iyang location
- [x] dapat always mag update iya location
- [ ] to lessen storage - delete the oldest location everytime mag add ug location if more than 10 ang iya location
- [ ] possibly use queue / others to periodically clear old patroller locations
## Citizen
### Update Incident Location
- [x] Route
- [x] Send location
- [x] update to timeline
- [x] send event to admin when location changes
## Admin
- [x] patroller marker
- [x] patroller dispatch on show page
- [x] marker contexts
- [x] marker behaviors
- [x] make requests not rerender the whole page
- [x] change citizen marker
- [x] change patroller marker
- [ ] put eta on patrollers
- [ ] navigation line from patroller to citizen

## Presentation
- [ ] prepare obs studio