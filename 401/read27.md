# Read: 27 - Intents, Activities, and SharedPreferences


* A task is a collection of activities that users interact with when performing a certain job. The activities are arranged in a stack—the back stack)—in the order in which each activity is opened. For example, an email app might have one activity to show a list of new messages. When the user selects a message, a new activity opens to view that message. This new activity is added to the back stack. If the user presses the Back button, that new activity is finished and popped off the stack. The following video provides a good overview of how the back stack works.
* The activities are stored in a back-stack. When a user starts to use an app, the activities are starting and push the current activity to the stack. Once the user finishes using the activity and moves to another one, the current activity will be popped from the stack and the new one will be pushed into the stack.
* If the user continues to press back button, it will continue backing to the previous activity until it reaches the home page or main activity with dropping each activity from stack.
* When the user is in the home page, the stack has only the home activity. Once the user presses back button, the home activity will be dropped from the back stack and at the end the task will be no longer exists.
* When the user is on the home page, the stack has only the home activity. Once the user presses the back button, the home activity will be dropped from the back stack and at the end, the task will be no longer exists.

* lunchMode attribute gives instructions on how the app is running.

#### launch mode Values:

* standard (the default mode).
* singleTop.
* singleTask.
* singleInstance.

##### The flags you can use to modify the default behaviour when starting a new activity are:

* FLAG_ACTIVITY_NEW_TASK
* FLAG_ACTIVITY_SINGLE_TOP
* FLAG_ACTIVITY_CLEAR_TOP

In manifest file, you can decide which activity should be the first one to execute when the app is running.

Save key-value data
SharedPreferences is one of the ways that is used to save data.
Calling one of these methods creates a SharedPreferences:
getSharedPreferences(): that it is used if you need multiple shared preference files identified by name.
getPreferences(): that is used if you need to use only one shared preference file for the activity.
To write to a shared preferences file, create a SharedPreferences.Editor by calling edit() on your SharedPreferences.
