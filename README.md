# Pre-work - *Simple Todo App*

**Simple Todo** is an android app that allows building a todo list and basic todo items management functionality including adding new items, editing and deleting an existing item.

Submitted by: **Mehak Channi**

Time spent: **5** hours spent in total

## User Stories

The following **required** functionality is completed:

* [x] User can **successfully add and remove items** from the todo list
* [ ] User can **tap a todo item in the list and bring up an edit screen for the todo item** and then have any changes to the text reflected in the todo list.
* [x] User can **persist todo items** and retrieve them properly on app restart

The following **optional** features are implemented:

* [ ] Persist the todo items [into SQLite](http://guides.codepath.com/android/Persisting-Data-to-the-Device#sqlite) instead of a text file
* [ ] Improve style of the todo items in the list [using a custom adapter](http://guides.codepath.com/android/Using-an-ArrayAdapter-with-ListView)
* [ ] Add support for completion due dates for todo items (and display within listview item)
* [ ] Use a [DialogFragment](http://guides.codepath.com/android/Using-DialogFragment) instead of new Activity for editing items
* [ ] Add support for selecting the priority of each todo item (and display in listview item)
* [ ] Tweak the style improving the UI / UX, play with colors, images or backgrounds

The following **additional** features are implemented:

* [ ] Incorporate a small dialogue box that will pop up before a user permanently deletes an item in order to ensure no item gets deleted by mistake (example message: “Are you sure you want to delete this item?”)
* [ ] Connect the user’s email address to the application so that a report can automatically be sent every morning to the user that will serve as a reminder of all of the items that have not yet been completed

## Video Walkthrough

Here's a walkthrough of implemented user stories:

<img src='http://i.imgur.com/link/to/your/gif/file.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />

GIF created with [LiceCap](http://www.cockos.com/licecap/).

## Project Analysis

As part of your pre-work submission, please reflect on the app and answer the following questions below:

**Question 1:** "What are your reactions to the Android app development platform so far? Compare and contrast Android's approach to layouts and user interfaces in past platforms you've used."

**Answer:** The Android app development platform provides a unique approach for designing and implementing mobile applications.  A variety of tools are available in order to effectively place buttons, input text, as well as entire list containers wherever required in the design, which therefore enhances the creative aspect of building a new app.  More importantly, all of the actions executed in designing the layout of the application are reflected in the corresponding XML source code, which makes the overall process of wireframing a new app quite simple and efficient.

In the past I’ve been exposed to development platforms such as Atom in order to create React Native applications for android devices.  Although this platform provides several useful packages and tools, it does not necessarily offer enough assistance in regards to planning the layout of an app.  The Android app development platform on the other hand is capable of creating a more accurate picture of what an app should look like in advance, which allows more time to focus on the actual functionality.   

**Question 2:** "Take a moment to reflect on the `ArrayAdapter` used in your pre-work. How would you describe an adapter in this context and what is its function in Android? Why do you think the adapter is important? Explain the purpose of the `convertView` in the `getView` method of the `ArrayAdapter`."

**Answer:** An adapter is responsible for displaying data by providing specific views for each item in the data set.  In the Simple Todo app for instance, this interface was utilized in order to ensure that all of the items that would be added to the todo list are instantly displayed according to their specified layout without any issues or interference.  An adapter is important because it not only effectively displays all the elements of a data set but it also provides instant access to those individual elements in a concise manner. 

The ArrayAdapter consists of a ‘getView’ method which assists in creating the views for a particular position of the list.  In order to properly implement the ‘getView’ method and correctly display the data, a parameter known as ‘convertView’ is passed into the ‘getView’ method.  The primary purpose of this parameter is to recycle old views as long as they are non-null and of the correct type.  In some cases however, if a particular view cannot be converted then a new view will automatically be generated.  

## Notes

Some of the challenges that I faced while building this app consisted of figuring out the proper syntax that corresponded to the latest version of Android Studio.  Due to the various updates involved in the new version, knowledge of the new syntax was essential in order to complete the rest of the application.  For instance, in order to implement persistence for the application, a third-party library needed to be installed.  However, when I initially attempted to incorporate this library by using the term ‘compile’, I received an error.  I eventually found out that the latest version of Android Studio no longer required the use of the term ‘compile’ and instead utilized ‘implementation’ for adding dependencies.

## License

    Copyright [2019] [Mehak Channi]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
