# Final-Assessment-arbaa

## Group members: Arba'a
### 1. Muhamad Aiman Bin Mohd Apendi 1915213
### 2. Ma Changhang 1927111
### 3. Muhammad Haikal Bin Razali 1921805

## Project Title: Implement NFC function into Chat App 

### Introduction
  Near Field Communication (NFC) functionality in a mobile phone application. NFC is a short-range wireless communication technology that enables contactless data exchange between devices. By integrating NFC into a mobile application, users can conveniently perform a variety of tasks such as making payments, exchanging information, and accessing secure areas.
  
   The NFC-based group chat application will revolutionize the way users connect and communicate within groups. By scanning NFC tags on other devices, users can effortlessly join group chats without the need for manual entry or complex setup procedures. This seamless process eliminates the barriers to entry and enhances user convenience. The integration of NFC technology simplifies the user experience, enabling individuals to connect quickly and easily with others in a group setting.

  Furthermore, the application will feature real-time messaging capabilities, ensuring instant and interactive communication within the group chat. Users will be able to exchange messages in real-time, fostering dynamic conversations and enabling efficient collaboration. The secure and private nature of the communication will be a priority, with encryption and authentication mechanisms implemented to protect user data and maintain privacy.

  The application's user interface will be designed with usability in mind. A user-friendly and intuitive interface will facilitate seamless navigation and interaction, enhancing the overall user experience. Clear and visually appealing design elements will guide users through the application's features, making it easy to engage with the group chat functionality.

  In summary, this project proposal envisions a group chat application that utilizes NFC technology for effortless joining of group chats. The application will prioritize real-time messaging, secure communication, and an intuitive user interface. By harnessing the power of Flutter, Dart, and various plugins, NFC Chat aims to provide a convenient and reliable solution for instant communication.


### Objectives
The main objectives of this group project are:
1. Develop a mobile application with NFC functionality for group chats.
2. Enable effortless joining of group chats by scanning NFC tags on other devices.
3. Incorporate real-time messaging capabilities within the group chat for seamless communication.
4. Prioritize security and privacy by implementing robust encryption and authentication mechanisms.
5. Create an intuitive and user-friendly interface for seamless navigation and effortless interaction.

In summary, the project aims to create a mobile application that utilizes NFC technology to simplify joining group chats, incorporates real-time messaging, ensures security and privacy, and provides a user-friendly interface.


### Features and Functionalities
1. NFC Tag Scanning: The application allows users to scan NFC tags present on other devices to initiate group chats. Once a tag is scanned, the user is seamlessly added to the corresponding group chat.
2. Group Chat Creation: Users can create new group chats and customize their names and settings.
3. Messaging: NFC Chat supports text-based messaging within group chats, enabling users to send and receive messages in real time.
4. User Management: The application provides functionalities for adding, removing, and managing group chat participants.
5. Notifications: Users receive notifications for new messages and chat invitations.
6. Authentication: NFC Chat integrates with Firebase Authentication to ensure secure user registration and login.
7. Cloud Storage: Firebase's Cloud Firestore is utilized for storing chat messages and user information securely.


### Project's Achievements
1. #### Completed Achievements:
   - Successfully developed a working Flutter chat app with Firebase integration.
   - Implemented essential screens: login page, registration page, home page, chat list page, and chat page.
   - Implemented user authentication using Firebase Authentication.
   - Integrated Firebase Cloud Firestore for storing chat messages and user information.
   - Developed functionalities for sending and receiving text-based messages in real-time within individual chats.
   - Implemented notifications to notify users about new messages.

2. #### Pending Achievements:
   - Group Chat Functionality: The ability to create new group chats and customize their names and settings is yet to be implemented.
   - NFC Tag Functionality: The feature to scan NFC tags to initiate group chats is pending.
   - User Edit and Participant Removal: The functionality to edit group chat details and remove participants from group chats has not been achieved.

To further enhance our project, we will focus on implementing the pending features mentioned above, such as group chat creation, NFC tag scanning, and user management functionalities. These additions will significantly improve the functionality and user experience of our chat app.



### Screen Navigation and Widgets Implementation:
In our Flutter chat app with Firebase, we will incorporate effective screen navigation and widget implementation to create a seamless and intuitive user experience. This section outlines our approach to handle the different screens and widgets within the application.

1. #### Screen Navigation:
To ensure smooth transitions between screens, we will leverage Flutter's Navigator class. By using named routes, we will define routes for each screen, including the login page, registration page, home page, chat list page, and chat page. This approach simplifies the navigation process and allows users to move between screens effortlessly. To navigate between screens, we will utilize the Navigator.pushNamed() method, while Navigator.pop() will enable users to move back to the previous screen.

2. #### Widgets Implementation:
Implementing various widgets is crucial for designing the different pages in our chat app. Here's how we plan to implement the key pages:

   a. Login Page: We will create a StatefulWidget for the login page, featuring user-friendly text fields for username and password input. Additionally, we will design intuitive buttons for login and navigation to the registration page. Within this widget, we will handle user input, perform necessary validation, and integrate Firebase authentication to authenticate users.

   b. Registration Page: Similar to the login page, we will create a StatefulWidget for the registration page. This page will include text fields for capturing username, email, password, and confirm password inputs. We will implement robust user input validation and leverage Firebase's user registration functionality to securely create new accounts.

   c. Home Page: The home page will serve as the central hub after successful login. It will feature a StatefulWidget with a thoughtfully designed user interface, showcasing chat list items, user information, and options for navigating to the chat list page and profile settings. To populate the UI, we will retrieve relevant user data from Firebase, ensuring a personalized experience.

   d. Chat List Page: We will create a StatelessWidget specifically for the chat list page. This page will present users with an organized list of their ongoing conversations. Each chat item will display the correspondent's name, profile picture, and the latest message. By retrieving chat data from Firebase, we will populate the UI accordingly. Additionally, we will implement smooth navigation to the chat page upon tapping a chat item.

   e. Chat Page: Our implementation will involve a StatefulWidget dedicated to the chat page. This page will showcase an intuitive user interface displaying chat messages, including the sender's name, message content, and timestamps. To enable real-time communication, we will leverage Firebase's Realtime Database or Cloud Firestore. By actively updating the UI as new messages arrive, we will provide users with a seamless and engaging chatting experience.

Throughout the development process, we will adhere to Flutter's widget-based structure, utilizing key widgets such as Scaffold, ListView, ListTile, TextField, RaisedButton, and more, to ensure a visually appealing and functional application.

By combining our screen navigation and widgets implementation strategies, we aim to deliver a user-friendly and immersive chat app, leveraging the power of Flutter and Firebase to create a seamless and enjoyable user experience.


### Sequence Diagram
  +--------------+           +----------------+         +-----------------+
  |  User A      |           |  User B        |         |  Firebase       |
  +--------------+           +----------------+         +-----------------+
         |                            |                          |
         |   Scan NFC tag             |                          |
         |--------------------------->|                          |
         |                            |                          |
         |    Join group chat         |                          |
         |--------------------------->|                          |
         |                            |                          |
         |   Retrieve chat data       |                          |
         |<---------------------------|                          |
         |                            |                          |
         |                            |                          |
         |     Send message           |                          |
         |--------------------------->|                          |
         |                            |                          |
         |                            |   Store message          |
         |                            |------------------------> |
         |                            |                          |
         |                            |       Notify             |
         |                            |------------------------> |
         |                            |                          |
         |    Receive message         |                          |
         |<---------------------------|                          |
         |                            |                          |
         |                            |                          |

### References
1. Chandler, N. (2012, March 14). What’s an NFC Tag? HowStuffWorks. https://electronics.howstuffworks.com/nfc-tag.htm
2. Sulaihi, M. (2022, March 28). How to build a chat application in Flutter with Firebase. LogRocket Blog. https://blog.logrocket.com/how-to-build-chat-application-flutter-firebase/
3. Muehle, C. (2022, October 10). NFC with Flutter. Flutter Community. https://medium.com/flutter-community/nfc-with-flutter-f8c3515cb0e0
4. Working with NFC in Flutter. (2022, September 2). Mews Developers. https://developers.mews.com/working-with-nfc-in-flutter/
5. flutter_nfc_kit | Flutter Package. (n.d.). Dart Packages. https://pub.dev/packages/flutter_nfc_kit
6. NFC. (2023, July 12). Flutter Awesome. https://flutterawesome.com/tag/nfc/

‌

