# Espresso

Espresso is a testing framework for Android to make it easy to write reliable user interface tests.

Espresso automatically synchronizes your test actions with the user interface of your application. The framework also ensures that your activity is started before the tests run. It also let the test wait until all observed background activities have finished.

It is intended to test a single application but can also be used to test across applications. If used for testing outside your application, you can only perform black box testing, as you cannot access the classes outside of your application.

Espresso has basically three components:

- ViewMatchers - allows to find view in the current view hierarchy

- ViewActions - allows to perform actions on the views

- ViewAssertions - allows to assert state of a view

The case construct for Espresso tests is to find the view first, perform an action on the view, and then validates an assertion.

We don't have to write our tests, because the is an API in AndroidX Test enables us to record our interactions with a device and add assertions to verify UI elements in particular snapshots.