# Convoo

Convoo started out as a conversational application, after exploring a number of databases and frameworks we settled on Firebase and Polymer,
as we explored Polymer a number of key web components for Convoo became evident. The plan is to build the web components we need and then
wire them together to form a final Convoo application. This vision has evolved to create a collection of reusable web components that will
allow developers to rapidly create real-time applications.

As a result of building the first set of components we learned that to truly understand the requirements for each web component and to ensure
they were interoperable we need to use them in real applications. This year we are going to create even more web components and launch a number
of MVP's to showcase them working together.

Upgrading new and existing components to Polymer 2 is eagerly anticipated.

Project ordering is described using a number wherever applicable, and * wherever the item is simply on the backlog.

## Web Components

### [Convoo-Fire]

A collection of elements that work with firebase.

#### 1 [Login-Fire]

A collection of elements for logging users in and out of an appliction.

- login-fire
- login-fire-social
- login-fire-form
- login-fire-button
- logout-button

#### 2 [Presence-Fire]

- An element that saves the presence of a user at a route and displays all other users at that route.

#### 3 [File-Fire]

An element that uploads files to firebase storage, images can be resized multiple times and a small base64 thumbnail created, returns two values a file path and if an image is uploaded a base 64 thumbnail.
Compatible with Form-Fire.

#### 5 [Form-Fire] 

A collection of elements for inserting text and image data to firebase database

- A form element that discovers inputs with an id of 'input-fire' and saves the input name and value along with the user's ID and a publish flag to the firebase database at a path matching the forms name. Data can bes saved as a doocument or as a list.
- A new input area that can preview markdown and show markdown tips. Data can bes saved as a doocument or as a list.
- An element to display a firebase list or document, displaying each list items or documents markdown if detected, the list can be ordered asc or desc. New items can be displayed at the top or the bottom. The number of items to be fetched can be limited, Content to be optionally stored locally for offline viewing. Content will be optionally fetched if The publish flag is set.
- CSV upload button to populate the same path as the form, the first row must contain matching names to the form inputs.

#### 6 [Report-Fire]

A collection of elements for reporting, displaying and unpublishing reported content

- An element that presents a button to allow a piece of content to be reported.
- An element that displays flagged content and the user who submitted the content. The contents publish flag can be toggled.

### [Webrtc-Components]

A collection of elements utilizing WebRTC for capturing and displaying audio/video.

#### 8 [Webrtc-Stream]

An element to capture the user's webcams audio and/or video steam.

#### 9 [Live-Video]

An element to display user webcam audio/video stream.

#### 10 [Socket-Connect]

An element to interface with socket.io.

#### 11 [Webrtc-Channel]

An element to manage webrtc audio/video streams accross a route.

- An element to specify TURN and/or STUN servers to be used.
- An element to publish the users audio/video stream to the current route.
- An element to display multiple other users audio/video streams for the current route.

### * [Social-Links]

An element that displays social links with SVG icons 

### * [More-Animations]

An element to add more animations to Neon Animations Runner.

### Planned MVP's

#### 4 [Photour]

An MVP that allows a user to sign in and upload images, the image will be displayed with a thumbnail and a link to the source.
Images containing pornographic content will be detected.

#### 7 [Spredd]

An MVP to allow users to create markdown articles with images, each article will have its own route. Users to have a profile page.

#### 12 [Cuple]

An MVP to build a site that randomly puts the user into a real-time video session with another user
 
### Contributions:

We continue to value and welcome all contributions and feedback to the Convoo components. And we would like to especially thank the following people:

- [LM450N] (Mason Louchart) - for significant contribution and refactoring [Login-Fire]
- [polinom] (Igor Polynets) - for contributions to the email + password component of [Login-Fire]

Join the conversation over at [Gitter]

   [Convoo-Fire]: <https://github.com/convoo/convoo-fire>
   [Login-Fire]: <https://github.com/convoo/login-fire>
   [Presence-Fire]: <https://github.com/convoo/presence-fire>
   [Social-Links]: <https://github.com/convoo/social-links>
   [File-Fire]: <https://github.com/convoo/file-fire>
   [Form-Fire]: <https://github.com/convoo/form-fire>
   [Report-Fire]: <https://github.com/convoo/report-fire>

   [Webrtc-Components]: <https://github.com/convoo/webrtc-components>
   [Webrtc-Stream]: <https://github.com/convoo/webrtc-stream>
   [Socket-Connect]: <https://github.com/convoo/socket-connect>
   [Webrtc-Channel]: <https://github.com/convoo/webrtc-channel>
   [Live-Video]: <https://github.com/convoo/live-video>

   [Social-Links]: <https://github.com/convoo/social-links>
   [More-Animations]: <https://github.com/convoo/more-animations>

   [Photour]: <https://github.com/Photour>
   [Spredd]: <https://github.com/Spredd>
   [Cuple]: <https://github.com/Cuple>

   [LM450N]: <https://github.com/LM450N>
   [polinom]: <https://github.com/polinom>
   [Gitter]: <https://gitter.im/convoo/General>
