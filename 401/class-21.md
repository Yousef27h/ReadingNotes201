# Intents, Activities, and SharedPreferences


## Tasks 

A task is a collection of activities that users interact with when performing a certain job.

The activities are arranged in a stack ( back stack ).

Starting from Android 7.0 (API level 24) and higher, when apps are running simultaneously , the system manages tasks separately for each window.

Activities in the stack are only pushed and popped from the stack only, push when activity starts and popped when the user leaves it using __Back__ button.

When all activities are removed from the stack, the task will disappear and will no longer be existing.

while task in the background, all its activities are stopped but the stack for the task remains intact.


## Shared Preferences

Shared preferences are used to read and write small collections of key-values pairs and save them.

To write to shared preferences we create `SharedPreferences.Editor` by calling `edit()` method on `SharedPreferences`.

To read from shared preferences we call methods such as `getInt()` and `getString()` providing the key for the value we want and a default value to return if the key isn't present.


