## CS472 Final Project January 2025: Contacts Manager Application
Description: Create a contacts management app where users can store and manage their contacts. Use the Node filesystem to store contact details (name, phone, email, etc.) in JSON files.

## Features:
* Add, edit, and delete contacts. Store contacts in a JSON file using the Node filesystem. 
* View a list of all contacts with details.
* Add a Speed Dial feature to bookmark important contacts, that will always appear on top of the contacts list.
* Search contacts by name, implement a real-time search filter that updates the contact list as the user types (filter contacts at frontend). 
* Enable users to export all contacts as `.vcf` files (vCard format) and download all exported `.vcf` files as a single compressed `.zip` file:
  * Use the `vcf` library to create `.vcf` files.
  * Use the `archiver` library to create `.zip` files.

## API Endpoints:
* `GET /contacts`: Fetch all contacts.
* `GET /contacts?export=1`: An optional `?export=true` query will export all contacts as `.vcf` files, compress and download as a `.zip` file.
* `POST /contacts`: Add a new contact.
* `PATCH /contacts/:id`: Update an existing contact.
* `DELETE /contacts/:id`: Delete a contact.

## File-Based Storage `contacts.json`:
```typescript
[
  {
    "id": 1,
    "name": "John Doe",
    "phone": "123-456-7890",
    "email": "john@example.com",
    "bookmark": false
  }
]
```

## Tech Stack: 
React for the frontend, Express for the backend, and Node filesystem for data persistence.
* Use React Router for navigation between pages.
* Leverage TailwindCSS for quick and responsive styling.
* Use Express API endpoints to handle CRUD operations and interact with the filesystem.
* Validate user inputs on both the frontend and backend to ensure data integrity. (Use `Zod`)

## Bonus (2 extra points)
* Deploy the frontend on a service like Netlify, Vercel, or any other similar service.
* Deploy the backend on a service like Heroku, Render, or any other similar service.
* Provide links to the deployed applications.

## Evaluation Criteria
* Does the application meet all specified requirements?
* Are all features implemented and working correctly?
* Is the code well-organized and easy to understand?
* Are best practices followed for both React and Express?
* Is the user interface intuitive and visually appealing?

### Notes
* A commit per feature is required, with a meaningful commit message.
* A daily push is required to track your code progress and measure your performance.
* You may only use and submit code to the repository provided by `maharishi-university` organization, do not submit code to your personal repository.
* Students are expected to be available on MS-Teams to receive calls and check on their progress every day from 10:00 AM to 12:00 PM, and 2:00 PM to 3:00 PM during the project.

## Need assistance?
Feel free to contact me any day between 10:00 AM to 12:00 PM, and 2:00 PM to 5:00 PM, except for Sunday. I’m available to assist all teams with all kinds of requests (system design, backend, frontend, fixing code bugs.. etc). The project is a learning experience and I want everyone to finish the project successfully and meet the course learning outcomes.

## Final Evaluation 
* The submission deadline is on Wednesday at 9:00 PM. Teams are expected to submit a screen recorded video that demonstrate the project features, and how to use the system. Do not show or explain your code patterns. Please send me the video URL on Teams. I might invite you to a meeting after the final exam to discuss your project if needed.
* It's advised that you submit your code on Wednesday morning, and prepare for your final exam.
* Your final exam will be on Thursday, from 10:00 AM to 12:00 PM, in the M115 classroom. Time management is key, finish your project early to allow time for exam preparation.

Good luck, and happy coding!

_Code Honor Submission Policy: Remember to respect the code honor submission policy. All written code must be original. You may not share any part of your code with other students. Code duplications will results to receiving NC for the final project. Presenting any code as one’s own work when it came from another source is plagiarism, which includes any matching patterns and code snippets, and will affect your grade. The use of AI is not permitted in this assignment. For more details, check the full course policies in the syllabus._
