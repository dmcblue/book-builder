# Book Editor Structure

## Broad Overview

- Persistence
- Server side (export and such)
- Backend API
- Frontend for editing
- Frontend for reading?

## Ideas for each item

### Persistence

#### Relational vs. Non-Relational

Books are large data items with lots of 'blob'-ish structures so in many ways 
NoSQL and its ilk are possible candidates. But I feel the intense number of relations
prohibit it from being used effectively.  I believe Relational databases would be best.

It's probably best not to assume this to be a performance power house out of the gates and just focus on getting the general ideas correct.

- MySQL/MariaDB 
    - Tried and true
	- handles complex relations well
	- continual development
	- Lots of devs
- PostGres
	- Don't know much about it, heard good things
- Git
	- The editing structure will need things like branches and pull requests. 
It may best to just use Git directly to handle this.  
	- https://stackoverflow.com/a/610315
    - git show 5f0252a12c5b9b51f21ee89af5b9c219cc083117:README.md
    - Grab XML from commit, and run parse over it.
- XML and Diff



### Backend / Server Side

- Golang
	- I've always wanted to actually use it for something
	- Con: I'm not great with module based code
- PHP
	- Always works
	- Con: not the fasted, especially with large data
- Java
	- Heavy duty
	- Performant
	- Con: its Java
- Node
	- ...

### Frontend

- Angular
	- Works well, well tested
	- Well known
- React
	- Less overhead than Angular
	- Redux
- Vue
	- Light weight

### General
- UTF8 Everywhere
