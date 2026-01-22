Code Structure
 User Class

Stores user credentials and quiz attempt history. Each user object maintains a record of all quizzes attempted, including score and time taken.

 Quiz Class

Represents an individual quiz. It stores the quiz title and a list of questions. Each question contains the question text, multiple options, and the correct answer.

 QuizSystem Class

This is the main controller class that manages users, quizzes, and quiz execution.

Data Management

users dictionary stores registered users

quizzes dictionary stores available quizzes

current_user tracks the logged-in user

 Functional Explanation
 load_default_quiz()

Preloads a default quiz so the system is ready to use without manual setup.

 register()

Allows new users to create an account by providing a username and password.

login()

Authenticates users using stored credentials and sets the active session.

start_quiz()

Allows logged-in users to select a quiz, attempt questions, and receive an automatically calculated score. The time taken to complete the quiz is also recorded.

 view_history()

Displays the logged-in user’s quiz attempt history, including scores and time spent.

 admin_add_question()

Provides an admin-only feature to add new questions to existing or new quizzes using a password check.

menu()

Displays a menu-driven interface that allows users to navigate through system features until exit.

 Program Execution

The program starts by creating an instance of the QuizSystem class and calling the menu() method to launch the application.
