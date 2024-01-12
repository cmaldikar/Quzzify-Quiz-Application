<p align='center'><img src='https://user-images.githubusercontent.com/46227193/133924458-d6f66df8-f0f8-4d56-951e-213200a2ad83.jpeg' width="300" ></p>

## What is it? ⛹️‍♂️
The project is a complete Exam Portal system built for educational institutions like schools and colleges. The portal serves as a single platform that can be used by all the professors and students, having their own set of work to be done. Following are the two levels of users along with the supported features that can be done by them in the portal:
* ***professor*** 👔

   * MCQ questions can be created/edited/deleted by professors which then further can be added to one or more question paper created by them.
   * The professor can create different groups of students as per their wish.
   * Exams can be created which can have a Question paper alloted to it by them.
   * Detailed analysis of result of all the quizzes attempted by the Student showing the top 5, bottom 5 and the average of the Student group 

* ***student*** 🧑‍
   * Can attempt exams allotted to them within the time constraints set by the professor
   * Can view their marks and solutions after completing the exam.
   * Have a list of all the exams completed and yet to be attempted in a single page 



## Cloning the Application in local ⬇️
1. Following software needs to be setup in the system for using the application in local
   * [python](https://www.python.org/downloads/)
   * [pip](https://pip.pypa.io/en/stable/installing/)
   
2. Open the project in any source code editor.


## Running the Application 🚚
### Local 💻
For running the project, navigate to the project directory and follow the following instructions:

* Type the following in the command line:
    ```sh
    python manage.py makemigrations
    python manage.py migrate
    python manage.py createsuperuser
    # this will ask for username, email(optional) and password. 
    # Enter some credentials to be used later for django admin functionality.
    python manage.py runserver
  ```

* Log on to [django admin site](http://127.0.0.1:8000/admin) using the superuser credentials
    * Click on **Groups** section and create 2 groups - ***Professor*** and ***Student***
    * Logout of the admin site and go to http://127.0.0.1:8000/ where the home page of the project will be rendered.

* Now any student/professor can login using their own credentials.


##### Credentials:
| User Type      | Username | Password |
| ----------- | ----------- | -----------|
| admin      | admin       | admin |


## Steps for creating a quiz:
* Login with professor credentials.
* Add some questions by clicking on Question Button.
* After adding all the questions click on Question Paper button and create a new question Paper by entering the question paper name and clicking on create button then selecting all the questions from the list.
* Then, Click on Student Group button on the professor dashboard to make a new student group by selecting the number of students by clicking Ctrl button and selecting multiple students who should give that particular quiz.
* After creating a Student Group, we go ahead a start creating an exam by clicking on Exams button. Here we select the Question Paper created along with the Student group created. Other details like Exam Name, Total Marks, Duration, Start Time and End Time should also be entered.
* The students selected in the student group while creating the exam can now give the quiz by logging in to their credentials and clicking on Exams button.
* Students can also see the result by clicking on the Results button.


## Built With 💕
* [Django](https://www.djangoproject.com/)
* [Django REST Framework](https://www.django-rest-framework.org/)
* Python
* HTML
* CSS
* JavaScript
* [Bootstrap](https://getbootstrap.com/)
* [Postman](https://www.postman.com/)
* [Visual Studio Code](https://code.visualstudio.com/)


## API info 👷
The APIs were built using **`Django`** and **`Django RESTFramework`**, which were further tested out using **`Postman`**. Some of the APIs tested can be found out

