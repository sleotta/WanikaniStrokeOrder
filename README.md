# WanikaniStrokeOrder

The aim of this project is to integrate Wanikani via a user's API key with the public kanji recognition api at https://kanji.sljfaq.org/.

Potential Technologies
- React Native (https://facebook.github.io/react-native/)
- npm (with yarn)
- React Native Sketch Canvas (https://github.com/terrylinla/react-native-sketch-canvas)
- SLJFAQ kanji API (POST: https://kanji.sljfaq.org/hw-17.cgi)

Planned stages

1. Get it working
  - Ability to add (and save locally) an API key
  - Ability to query the Wanikani API for a list of (burned) kanji
  - Ability to draw a kanji and save it as a bitmap
  - Ability to send that bitmap through to SLJFAQ and get a list of potential Kanji
  
 2. Local random quizes
  - Generate a list of 5 kanji readings and meanings
  - Create a quiz from those with the following structure
    - Question is asked (e.g. What kanji means fire? (readings: ひ, カ)
  - User draws a kanji and it is sent to SLJFAQ for matching
  - User selects a kanji from teh list of matches
  - Result is saved and a score is given at the end
  
3. Local stored quizes.
  - Have a file on the user's phone which stores their quiz results
  - Use this as a kind of SRS system
  - Create assessed quizzes based on this SRS

4. Use a db
  - Store users against their API key in a database
  - Use the db for storage of quiz results so that users can access their results from any device
