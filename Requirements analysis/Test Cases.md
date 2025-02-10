Test Case № 1:
Title: Verify navigation to the Trainings Tab from Personal Plan
Preconditions: Open the app.
Steps:
1. Go to the Personal Plan screen.
2. Tap on the Do Your Workout card.
Expected Result: The user is navigated to the Trainings Tab.

Test Case № 2:
Title: Verify that Today’s Activity contains between 1 and 3 workouts
Preconditions: Open the app.
Steps:
1. Navigate to the Trainings Tab.
2. Check the Today’s Activity block.
Expected Result: Today’s Activity block contains 1 to 3 recommended workouts based on the user’s selected activities.

Test Case № 3 (Negative):
Title: Verify behavior when Today’s Activity block has 0 workouts
Preconditions: Open the app.
Steps:
1. Go to the Personal Plan screen.
2. Check if the Do Your Workout card is displayed.
Expected Result: If the card is missing, the user should not be able to access the Trainings Tab through it.

Test Case №4
Title: Verify the correct subtitle for 1 chosen activity
Preconditions: 
1. Open the app
Steps:
1. Select one activity on the activity selection screen.
2. Navigate to the Trainings Tab.
Expected Result: The subtitle is: "Get daily workouts tailored to your goal and interest in [Chosen Activity #1]."

Test Case №5
Title: Verify the correct subtitle for 2 chosen activities
Preconditions: 
1. Open the app
Steps:
1. Select two activities on the activity selection screen.
2. Navigate to the Trainings Tab.
Expected Result: The subtitle is: "Get daily workouts tailored to your goal and interests in [Chosen Activity #1], [Chosen Activity #2]."

Test Case №6
Title: Verify subtitle update when all workouts are completed
Preconditions: Open the app.
Steps:
1. Complete all recommended workouts.
2. Check the Recommended for You section.
Expected Result: The subtitle updates to: "All workouts done! For an extra challenge, check out the workout library below."

Test Case №7
Title: Verify that the "Do Your Workout" card is marked as completed after all workouts are done
Preconditions:
1. Open the app.
2. Navigate to the Personal Plan screen.
Steps:
Complete all recommended workouts.
Expected Result: The Do Your Workout card is visually marked as completed.

Test Case №8
Title: Verify that the "Do Your Workout" card is clickable and redirects to the correct screen
Preconditions: Open the app.
Steps: Tap anywhere on the Do Your Workout card.
Expected Result: The user is navigated to the Workout Preview Screen.

Test Case №9 (Negative):
Title: Verify behavior when no activities are selected 
Preconditions: Open the app and don't select any activities.
Steps: Navigate to the Trainings Tab.
Expected Result: The Recommended for You section should be hidden or display a message like "No recommended workouts available."

Test Case №10 (Negative): 
Title: Verify behavior when subtitle does not update after completing a workout	
Preconditions: Open the app  
Steps: 
1. Complete one workout.
2. Check the subtitle Recommended for You.
Expected Result: The subtitle should correctly update to "Great job! [N] more workout left."

Уточнення: 
1. Додати дизайн-макети Trainings Tab та блок "Today’s Activity"
2. Чи можна змінити кількість обраних користувачем activity та їх типи? На якій вкладці?
