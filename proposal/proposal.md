# Project Proposal
QuizIt! A Quizlet clone that allows you to create groups and add your friends or study buddies to them to share sets of flashcards. 
1. What tech stack will you use for your final project? We recommend that you use
React and Node for this project, however if you are extremely interested in
becoming a Python developer you are welcome to use Python/Flask for this
project.

  - I will use Node and React for the frontend and Express and Postgres for the backend.

2. Is the front-end UI or the back-end going to be the focus of your project? Or are
you going to make an evenly focused full-stack application?

  - I'm hoping to make an evenly focused full-stack application.

3. Will this be a website? A mobile app? Something else?

  - It will be a web application. 

4. What goal will your project be designed to achieve?

  - The app will allow users to create/edit/delete sets of online flashcards and quiz themselves on topics they wish to learn. It will be like a Quizlet clone, except you can create groups and add people to them to share a set of flashcards. 

5. What kind of users will visit your app? In other words, what is the demographic of
your users?

  - The target demographic of this app is mainly students of any age or subject. Whether you're studying for your next interview or test, everyone needs to rep flashcards sometimes!

6.  What data do you plan on using? How are you planning on collecting your data?
You may have not picked your actual API yet, which is fine, just outline what kind
of data you would like it to contain. You are welcome to create your own API and
populate it with data. If you are using a Python/Flask stack are required to create
your own API.

  - I will create my own API and the users will populate the data by creating sets of flashcards. Flashcards will consist of the front text, back text, and pictures if the user desires. 

7. In brief, outline your approach to creating your project (knowing that you may not know everything in advance and that these details might change later). Answer questions like the ones below, but feel free to add more information:
  - What does your database schema look like?
    - There will be a table for users, flashcards, flashcard sets, and groups at least. Possibly user history? Tables like users_groups and flashcard_flashcardSets could be helpful. Will think about this in more detail in Step 3.
  - What kinds of issues might you run into with your API? This is especially
important if you are creating your own API, web scraping produces
notoriously messy data.
    - Will have to be careful setting up Express API to query database. Will not be very populated at first, maybe need to create an example set of cards? Maybe a global search for public sets of cards so the app doesn't seem empty when a new user registers?
  - Is there any sensitive information you need to secure?
    - No sensitive information other than user password, which will be hashed and stored securely using bcrypt.
  - What functionality will your app include?
    - Allow users to login/signup to browse sets of flashcards or groups that contain sets of flashcards. Allow users to create their own sets of flashcards and invite their friends. Allow users to quiz themselves on flashcards maybe? Like Quizlet does. 
  - What will the user flow look like?
    - Users log in to their dashboard, which could show 3-5 recently browsed sets if applicable? Else, it says "start studying" and prompts you to create a new set of flashcards or search for existing groups/flashcards. Navbar on top to lead to popular pages (user dashboard, groups, public flashcard sets, own flashcard sets?). Users can click through flashcards to test themselves and at the end it prompts user to reshuffle and repeat or quit studying. Maybe include thumbs up/thumbs down to let user indicate if they got the card right or wrong? More difficult cards will appear more often? (Could include difficulty score where thumbs up is a +1 and thumbs down is a -1)
  - What features make your site more than a CRUD app? What are your
stretch goals?
    - Users can interact with flashcards and add people to groups to interact with flashcards. Stretch goals include some kind of difficulty algorithm (maybe just an integer difficulty score?), user-selected themes throughout the app to make is more visually appealing, inviting friends by email, notifications on top informing a user they've been invited to a group or their join request was approved by an admin. If too difficult, can also implement passwords for private groups or flashcard sets. 