# form

## sunday
- date
- preacher
- song leader
- worship leader
- tithes and offering amount
### preaching
- sermon title
- scripture
## wednesday
- date
- preacher
- song leader
- prayer leader
- worship leader
- tithes and offering amount

## attendance
- name

## visitors
- name

### notes
- pink
- avocadp


# Database Schema
## Member
{
	id: String unique,
	name: String,
	birthday: Date
}
## Attendance
{
	id: String unique
	date: Date,
	amount (name pending, pwede ra pud iisa lang): {
		tithe: float, 
		offering: float,
	} 
	sermon: {
		preacher (Essentially a reference to member, but includes name para dali ma query): {
			id: member_id,
			name: String
		},
		title: String,
		scripture: String	
	},
	 worship leader (Member Reference): {
		 member_id,
		 name: String,
	 },
	  song leader (Member Reference): {
		 id: member_id,
		 name: String,
	 },
	 songs: Array<String>
	 attendance: Array<{
		 id: member_id,
		 name: string
	 }>,
	 visitors (after mag submit sa form, i add dayun ang visitors sa members) : Array<{
		 name: string,
		 birthday: date
	 }>,
	 birthdays: Array<{
		 id: member_id,
		 name: string,
		 birthday: date,
	 }>
}