### EY Fraud detection website (summer intern)

### The task

Develop a fraud detection website, along with a dynamic dashboard, that stores metrics even after the webpage is closed.

Users should be able to:

- Upload documents and view them
- Submit these documents and get a response if the documents are fraud or not
- Decide if this decision by the machine was correct or not.
- See an interactive dashboard that displays different stats such as: false positives, frauds, total documents reviewed, etc.

## My process

I used bootstrap to structure this website. The whole website is inside a large container class. I started with first making a navbar that always sticks to the top, and a side bar as well. Then I structed all these websites such that they are responsive on tablet size screens as well. I made use of JavaScript to create the functions to be used on the website. Used it to make the refresh, submit, fraud, not fraud buttons. The number of clicks on the evaluation page is updated in real time on the dashboard page, depending on which button is clicked. One challenge was how to save the JavaScript variable even after the page has been refreshed. This was solved by using localstorrage. After a document has been evaluated, a message pops up saying that "your response has been recorded, please click on the refresh button." The user can then select his next document. The dashboard option on the sidebar displays charts and stats about the current documents reviewed. The stats are only erased when the user clicks reset, otherwise not.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- JavaScript
- JavaScript Libraries
- Bootstrap

### Important notes:

-Need to look for a better font
-Need to create an undo button to reverse the last selected response.
-The reason for document being fraud is selected randomly, needs to be connected the backend code so that it displays the correct reason.
-gettingdata.js is responsible for sending data across the two webpages (evaluation to dashboard)
-Imported chart.js
- The response of fraud or not fraud from the user won’t be recorded and displayed on the dashboard UNLESS a file has been selected and upload button was clicked. Only then the user can click, either button, only once. 
- The undo button could be made by pushing every instance of the variable by using .push() and then removing the most recent elemt from the array
using .pop() and then displaying the last element of the array.

### Continued development

The reason for the documents being fraud is hard coded, hence it needed to be connected to the actual OCR reader and fraud detection code. The website could also be made mobile responsive, however it completely responsive above 700px, which is table sized and above. The website can also be made more aesthetic.

### Useful resources

https://www.w3schools.com/
https://stackoverflow.com/

## Author

Madhav Kapoor
LinkedIn: www.linkedin.com/in/madhavkapoor28
Email: madhavmkapoor@gmail.com

