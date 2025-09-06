# Authentication
- post - /api/admin/login
	- email
	- password
- post - /api/admin/logout
- get - /api/admin/profile

# Role
- get - /api/admin/role
- get - /api/admin/role/{id}
- post - /api/admin/store
	- name
	- hex

# Sector
- get - /api/admin/sector
- get - /api/admin/sector/{id}
- post - /api/admin/sector/store
	- name
	- region
	- longitude
	- latitude
- post - /api/admin/sector/{id}/store
	- name
	- region
	- longitude
	- latitude

# Officers
- get - /api/admin/sector/{sectorId}/officer
- get - /api/admin/sector/{sectorId}/officer/{officerId}
- post - /api/admin/sector/{sectorId}/officer/store
	- name
	- email
	- password

# Patrollers
- get - /api/admin/sector/{sectorId}/patroller