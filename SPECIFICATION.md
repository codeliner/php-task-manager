# PHP Task Manager - Specifications

1. [Introduction](#specs)
	* [The rules](#specs-rules)
	* [Project definition](#specs-project)
	* [Task definition](#specs-task)

## <a name="specs"></a> Introduction

For this project, we need to create a tool to manage **Tasks** that will
be given for any kind of professional. To meet their needs, we need to
organize **Tasks** into **Projects**.

We need to implement a control panel for each user, and a form where
new users can signup and create their projects.

From this panel, a **User** can create a **Project**. They can invite
other **Users** to participate in their **Projects**.

### <a name="specs-rules"></a>The rules

* Each **Project** CAN have many **Users**.

* A **User** CAN create, delete, edit and change the status of any
**Task** that they are assigned to.

* Any **User** CAN create a **Task**

* A **Task** CAN be assigned to an **User**.

* Each **User** CAN assign to himself a **Task** that have not been assigned yet.

* Just the **User** with the *role* "owner" can assign any **Task** to any
**User**.

* A **Task** MUST be in one of the following statuses: "To do", "Doing"
and "Done".

* A new **Task** is created with status  "To do".

* A **Task** CAN change its status, just when they have an **User** assigned
to it.

### <a name="specs-project"></a> Project definition

Each **Project** MUST contain at least:
>
* A *label* to describe its name
* A *creation timestamp*
* An **User** with the *role* "owner"

Each **Project** CAN contain:
>
* A **Task**.
* One or more **Users** with any *role*


### <a name="specs-task"></a> Task definition
Each **Task** MUST contain at least:
>
* A *label* to describe its name.
* A *description* to tell us its requirements for completion.
* A *creation timestamp*.
* A *status*.

Each **Task** CAN contain:
>
* An **User** assigned to it.
* A *last change timestamp*.
