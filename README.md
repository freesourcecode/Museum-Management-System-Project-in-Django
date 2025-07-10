# Museum Management System Project in Django with Source Code

The **Museum Management System Project in Django** created based on python, Django, and SQLITE3 Database.

The **Museum Management System**, the museum’s manager has access to add and update privileges for artifacts, artists’ information, and employee and department data.

The manager can use the portal to make the necessary adjustments and additions.

Visitors can create an account on the internet and purchase museum tickets in advance.

After signing up, the user can log in using the same credentials and view the museum’s items as well as information about the museum’s departments and artists.
>[!NOTE]
> To start creating a **Museum Management System Project in Python Django**, makes sure that you have PyCharm Professional IDE Installed in your computer.

## Admin Features: Museum Management System in Django

* **Login Page**

The page where the system administrator enters their system credentials in order to gain access to the system’s administrative side.

* **New Employee Page**

This is the page where an administrator can add a new employee.

* **Employee List**

The page on which the list of employee can be viewed, modified, or deleted.

* **New Artist Page** 

The page to which an administrator can add new artist.

* **Artist List**

The page on which the list of artist can be viewed, modified, or deleted.

* **New Artifact Page**

The page to which an administrator can add new artifact.

* **Artifact List**

The page on which the list of artifact can be viewed, modified, or deleted.

* **New Department Page**

The page to which an administrator can add new department.

* **Department List**

The page on which the list of department can be viewed, modified, or deleted.


## Museum Management System in Django: Visitor Features

* **Home Page**

When visitor visit the website, this is the system’s default page. 

* **Register Page**

The page where new visitor created their login credentials for the website.

* **Login Page**

Visitor enter their website credentials on this page to gain access to all of the website’s features.

* **Manage Profile Page**

The page where the visitor can update their own profile information.

* **Book Ticket Page**

The page where the visitor can book a ticket to the museum.

* **Send Feedback**

The page where the visitor can send feedback to the admin about in museum.

## How to Create a Project Museum Management System in Django?

Here are the steps on how to create a Museum Management System Project in Django with Source Code.

1. **Open file**.

Open “pycharm professional” after that click “file” and click “new project”.

![image](https://github.com/user-attachments/assets/3bb6159a-4b13-48e6-af99-fa7cb168a16d)


2. **Choose Django**.

Next, after click “new project“, choose “Django” and click.

![image](https://github.com/user-attachments/assets/ed6616f1-9f4f-4d56-bdbd-8a0f5c96fc76)

3. **Select file location**.

Then, select a file location wherever you want.

4. **Create application name**.

After that, name your application.

5. **Click create**.

Lastly, finish creating project by clicking “create” button.

6. **Start Coding**.

Finally, we will now start adding functionality to our Django Framework by adding some functional codes.


## Functionality and Codes of the Museum Management System Project in Django with Source Code

* **Create template for the book ticket form in Museum Management System in Django**.

In this section, we will learn on how create a templates for the book ticket form. 

To start with, add the following code in your book_ticket.html under the folder of /templates/.

```
{% load static %}

<!DOCTYPE html>
<html>
<head>
	<title>Book Ticket</title>
	 <link rel="stylesheet" href="{% static "css/style.css" %}" /> <!-- CSS -->
</head>
<body background="{% static "images/visitor.jpg" %}">
	<center><h1 style="color: black; background-color: yellow;opacity: 60%;"> Hello , you are in Ticket Booking !!! </h1></center>
  <br><br><br>

	<center>
   <div style="background-color: lightblue;">
   <form  action="/ticket_book/" method="POST">{% csrf_token %}

      <label class="label">Visit Date&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</label>
      <input type='text' name='date' required value={{date}}>
      <br>(YYYY-MM-DD)<br>
      <label class="label">Number of Tickets</label>
      <input type='number' name='number' required value={{not}}>
      <br>
      <label class="label">Type(N/S)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</label>
      <input type='text' name='type' required value={{type}}>
      <br><br>

      <input name='submit' type='submit' value='Book Ticket' style="background-color: blue;"><br>
      
    </form> 
  </div> 
  </center>

    <br><br>{{error}}
	
</body>
</html>


```

* **Create template for the feedback form in Museum Management System in Django**.
In this section, we will learn on how create a templates for the feedback form.
To start with, add the following code in your feedback.html under the folder of /templates/.


```
{% load static %}

<!DOCTYPE html>
<html>
<head>
	<title>Add Feedback</title>
	 <link rel="stylesheet" href="{% static "css/style.css" %}" /> <!-- CSS -->
</head>
<body background="{% static "images/visitor.jpg" %}">
	<center><h1 style="color: black; background-color: yellow;opacity: 60%;"> Hello , you are in Feedback !!! </h1></center>
	<br><br><br>

	<center>
		<div style="background-color: lightblue;">
		<form  action="/feedback/" method="POST">{% csrf_token %}

      <label class="label">Date of visit&nbsp;&nbsp;&nbsp;</label>
      <input type='text' name='date' required value={{date}}>
      <br>(YYYY-MM-DD)
      <br>
      <label class="label">Type of ticket</label>
      <input type='text' name='type' required value={{type}}>
      <br>
      <label class="label">Feedback&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</label>
      <input type='text' name='feedback' required value={{feedback}}>
      <br><br>

  	  <input name='submit' type='submit' value='Add Feedback' style="background-color: blue;"><br>
  	  
    </form>
	</div>
	</center>

    <br><br>{{error}}
	
</body>
</html>

```

### 📌 Here's the full documentation for the [Museum Management System Project in Django](https://itsourcecode.com/free-projects/python-projects/museum-management-system-project-in-django-with-source-code/)

