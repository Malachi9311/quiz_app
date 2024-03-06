# A Simple JS Quiz Application

- ### HTML structure
  - Project will be contained in one single app_div within Body tag.
  - Heading of the project inside app_div
  - Nest a Quiz_div within, this will contain question and answer buttons inside
    - Create h2#question -> Question tag
    - Create div#answer-button -> dynamically create 4 button tags
      for each answer (Psuedo buttons) using JS later (Put 4 buttons in the meantime for styling)
    - Create button#next-btn -> move to the next question.
- ### CSS
  - Wildcard
    - margin and padding == 0
    - font == Poppins
    - Box-sizing == border-box
    - body tag background color
  - .app_div
    - max-width == 600px
    - margin == 100px auto 0
    - padding == 30px all around
    - border radius == 4px
    - h1 tag styling with border-bottom == 1px and padding bottom == 10px
  - .Quiz_div
    - 20px padding
    - h2 tag styling
  - .btn_buttons
    - 100% width
    - text-align == left
    - general styling
    - cursor == pointer
  - #next-btn
    - width == 150px
    - margin == 20px auto 0
    - display == none (Will be changed by eventListener)
- ### JavaScript
  - Questions (Array of objects)
    - Contains an object of 1 question and 4 possible answers
    - question : String
    - Answers : Array of objects
    - text: String, correct: Boolean
  - Make instances of elements by ID
    - questionElement -> change Question dynamically.
    - answerButtons -> Make answers, put into buttons.
    - nextButton -> Display "Next" button after selecting first answer.
  - ## Static variables
    - Current Question Index == 0
    - Total Score == 0
  - ## Functions
  - startQuiz()
    -> Start a new quiz session
  - showQuestions()
    -> Move to next question with given answers.
  - resetState()
    -> Reset state
  - selectAnswer()
    -> add eventlistener to select correct answer
  - showScore()
    -> Display final score once quiz is finished.
  - handleNextButton
    -> What happens when next-btn is clicked
  - nextButton.eventlistener()
    -> call handleNextButton()/startQuiz()
