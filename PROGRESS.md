# Progress Log

## Overview

This file tracks the development progress of the Interactive Handtracking and storing in a Database project, including achievements, updates, challenges, and solutions.

## Updates

**22-11-2024**

- Set up initial commit.
- Set up hand tracking with the use of mediapipe.
- Set up left hand zone tracking.
- Set up OSC Out to Resolume Arena.

**29-11-2024**

- Set up Database with Supabase.
- Starting Post to Database TOX.
- Challenged by webclient, convert and chopexecute.

**05-12-2024**

- Fixed Python code to Post to Database.
- Achieved correct Post of data to database, posting different hands.

**26-12-2024**

- Updated Posting of data to database, cleaning flow of components.
- Added a session timer, each time the camera stops tracking the hand a delay sets and a new session is started, marking differences in users.
- Users tried the handtracking and post to database.
- Results: 2 sets of data, from a 12 year old child and 48 year old man.
- Cuncluded childs will play way faster with their hands to acchive results then adults, they take more time to understand the function.
- Imorting JSON from Supabase SQL to Touchdesigner file to visualise the data.

**27-12-2024**

- Tested different types of visualising the data.
- applied conventions to session_trigger component, Visualising_DATA, Post_To_Your_Database and Handtracking.
- Progress.md and Conventions.md documentation added and updated.
