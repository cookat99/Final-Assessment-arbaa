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

### Screen Navigation and Widgets Implementation
Navigation flow
                    +-------------+
                    |  StartPage  |
                    +-------------+
                           |
                           |
                           v
                   +----------------+
                   |   LoginPage    |    TextField and MyButton(onTap)
                   +----------------+
                   |  RegisterPage  |    TextField and MyButton(onTap)
                   +----------------+
                           |
                           |
                           v
                   +----------------+
                   |  HomeScreen    |    ElevateButton(ontap), BuildList
                   +----------------+
                   |  ChatListPage  |    onTap, BuildList
                   +----------------+
                   |  ChatPage      |    TextField and Icon
                   +----------------+

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

