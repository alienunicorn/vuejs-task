# Frontend Development Test

[![Codetribe](https://codetri.be/banner.png)](https://codetri.be)

Goal of this project is to test basic understanding of frontend development , from project setup , preprocessor and building configuration to basic manipulation of data inside a web application. Your task will be to build a student maangement web application that will be able to perform some of basic CRUD operations, add student to a student list, move student from that list to one or more student groups, remove them from those groups etc.

## Required tools
  - Javascript framework of your choosing (**Angular**, **Vue** (we like this one but feel free to choose your own))
  - Style preprocessor (**Sass**, **Less**, **PostCSS** etc)
  - **Git** installed
  - Javascript package manager (**npm** , **bower** or **yarn** (you can use multiple package managers inside a single project but avoid this , if there is a lib you want to use on bower, but all your libs are on npm, found a lib similar to one you had choose inside npm package repository)

## Project synopsis
This web app should contain tab menu on the top that can easily switch routes from page 1 to page 2, only one tab can be active.

**Page 1: Overview of the students on the platfrom**
This page should contain:

- On the left side there should be two input fields: Student First & Last Name, and button Add student that will execute a function and add that student the student table. New student should have a unique id once it's created. This id should be auto generated by either by using a library or using localstorage and incremeting a single field that will serve as an id everytime new user is created. Don't hardcode this.
- On the right side there should be a table that list all the students on the platform. Table should contain a select menu with sorting capabilities:
-- Sort students by name from A-Z
-- Sort students by name from Z-A
-- Sort students by id from lowest to highest
-- Sort students by id from highest to lowest

**Page 2: Overview of the groups and students on the platfrom**
This page should contain:
- Table on the left that shows **all groups** on the platform
This table should list all groups on the platform and inside every group should be overview of all students in this group. Students can be removed from the group by clicking on the remove button. Table should contain a select menu with sorting capabilities:
-- Sort groups by name from A-Z
-- Sort groups by name from Z-A
-- Sort groups by id from lowest to highest
-- Sort groups by id from highest to lowest

- Table on the right that shows **all students** on the platfrom
This table should list all students. Table should contain a select menu with sorting capabilities:
-- Sort students by name from A-Z
-- Sort students by name from Z-A
-- Sort students by created timestamp from lowest to highest (timestamp should be saved once the user is created with the rest of the user data)
-- Sort students by created timestamp from highest to lowest (timestamp should be saved once the user is created with the rest of the user data)

- Button: **Add new group**
This button will open a modal that can add new group to the platform. This modal should have one input field: Group name , and button Add group that will execute a function and add that group to the groups table. New group should have a unique name once it's created.

- Button: **Move student to group**
This button will open a modal that should have two input fields: select menu that list all users and select menu that list all groups on the platform. **NOTE**: Single user can exist in multiple groups!

**You can choose the following data storage options listed from easiest to hardest:**
- Local storage inside browser
- JSON file
- **extra bonus** firebase integration

**Validations that should be implemented:**
- Unique user id
- Unique user id in group
- **bonus** input validations
    - the validations to implement are completely up to you. **NOTE**: this task is all or nothing - if you implement validations on one field - they should be implemented on all others as well

## Extra bonus tasks
- Implement drag and drop functionality to add student to the group
- Implement drag and drop functionality to reorder students in the student list
    - **NOTE** this order should also be stored
- Implement drag and drop functionality to reorder groups
    - **NOTE** this order should also be stored
- Key bindings on all actions (example: enter should submit the modal, esc char should close the modal etc.)
- Implement edit functionality for users, where you can update first and last name of the user. Once user is edited store update timestamp. Then expand users table to sort users by edit time as well. Once user data is changed update all tables that have that user.

## Design files:
[![Codetribe](https://codetri.be/final1.png)](https://codetri.be/final1.png)
[![Codetribe](https://codetri.be/final2.png)](https://codetri.be/final2.png)
