# Hand Tracking Data

## Project Overview

This Touchdesigner project is a Interactive Hand Tracking project where players can move their hands in front of a webcam which depending of their hand location will trigger an animation in Resolume Arena. This hand tracking movement is aggregated through a database using **Supabase**. This data is then imported as a JSON using SQL coding, and visualized in the Touchdesigner file itself. showing the speed a child moves their hand in comparison with adults.

## How to Run

1. If you don't have Mediapipe installed yet on your machine you'ill need to instal it first in your components.
2. If you don't have Resolume Arena you can download a free version on their website.
3. Open de Touchdesigner file `INTERACTIVE_DATA`.
4. Drag your MediaPipe from your components and turn off: Detect Faces, Detect facial landmarks, Detect poses, Detect objects, Classify images and Detect image embeddings.
5. Connect the normalized_data out to the HANDTRACKING Container.

**Interactive handtracking**
With these steps your hands can be tracked and animations will be triggered in Resolume Arena.

# If You Wish to Develop

## For Aggregated data using a Database

5. Link The HANDTRACKING OUTs to the corresponding CHOPs, these will be linked to the rest of the Notes.
6. In the POST_TO_YOUR_DATABASE Container, in the post_json DAT you can change the url of your Database and set the apikey.
7. change the convert and channelJSON DATs to your needs.
8. to run the script right click the post_json and press Run Scripts

**Optional**
If you want the handtracking to Post each time a hand is placed in a new zone you can unable the Bypass of the chopexecute DAT underneath the toConvert DAT.

## To Visualize the data using your database

9. If everything went correctly your data should be stored in your database.
10. Using SQL code like this example:

SELECT "session_id" FROM "TD_Interactivity";
SELECT \* FROM "TD_Interactivity" WHERE session_id = '1';

You can extract data from each session. 11. Export/Copy the table on your machine 12. In the Touchdesigner File you can go to the blue **DATA VISUALING** section and import/paste your JSON in the JSON_TABLE DAT 13. In the Visualising_DATA Container you can change things depending on your needs of visualasation. 14. in the hands_1280x720 TOPs you can import an other image to your liking and change it's background color in the Containers linked after it.

## Folder Structure

- `Assets/`: All images or video's u'd need.
- `TABLE_FILE_IN/`: All CSV,JSON, other data files.

## Documentation

All documentation can be find in the folder or Github.

## References

- **Webclient**: Touchdesigner Forum was used for the Webclient Container to Post to the Database [Forum Link](https://forum.derivative.ca/t/webclient-dat-simple-put-and-post/229814).
- **Supabase Database**: Used Supabase Database for collecting the hand tracked data [Website] (https://supabase.com).
- **MediaPipe**: Using the MediaPipe Plugin form Torinmb [Plugin](https://github.com/torinmb/mediapipe-touchdesigner).

## Attribution & License

This project is developed by **Louis-James Pouleur**.

This project is licensed under the MIT License. See the full license text in the LICENSE.md file.
