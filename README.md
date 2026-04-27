Introduction

The City Scenario project was carried out with C++ and OpenGL, and its modular functions for each object like buildings, cars, trees, birds, and clouds were created. Triangle fan, translation, rotation, and sine animation were used to create smooth and interactive effects. The final scene includes a vibrant transition from day to night, moving cars, birds, and trees that sway, and clouds that float, showcasing the advances in real-time rendering and making animated objects visually appealing.	

Project Setup

The project was executed in C++ with the tools of Visual Studio / Code::Blocks and worked on OpenGL and FreeGLUT for the purpose of rendering. The double buffering technique was used to set the application window and thereby achieve smooth animation. The use of gluOrtho2D facilitated the setting up the viewport, thus defining a 2D coordinate system that completely covers the scene, granting a uniform reference for the positioning and displacement of objects.

Object Development

Buildings: To create each building, rectangles and quads were used ultimately to make it look 3D. Windows change color through interpolation (Lerp) as an indication of lights on and off during the transition from day to night.

Car: The car is made up of rectangles for the body and cabin, whereas the wheels are filled circles created by using the Triangle Fan technique. The rotation of the wheels is also applied to show the realistic movement of the car along the road.

Trees: The trees consist of the rectangular part added with a circular one that is the foliage. The foliage is given a little horizontal swaying based on sine which in turn adds a natural animation effect to the scene.

Birds: The birds are represented by very simple line-based shapes; the movement of the wings is caused by a sine function that controls vertical oscillation thus imparting a realistic flying motion.

Clouds & Sun/Moon: The clouds and the celestial bodies are represented by multiple overlapping circles. The clouds example is that they are constantly moved across the sky to imitate natural drifting, while the sun and moon are turned on and off in accordance with the day-night cycle.

Animation & Transformations

Translation: It was used for cars, birds, and clouds to instantly transfer them across the scene in a smooth manner.

Rotation: The wheels of the car turn to show movement thereby increasing the realism.

Sine-based Motion: It is a technique that is widely used for subtle natural effects such as bird wing flapping and tree foliage swaying.

Color Interpolation: It makes gradual sky transitions from day to night and dynamic lighting changes in the windows of the building which makes the whole view more beautiful.

Interactive Features

Keyboard Controls: By pressing 'N', users can switch on Night Mode and by 'P' can control the animation to Pause or Resume at their will, thus allowing interactive control of the scene.

Real-Time Updates: A timer-based loop (glutTimerFunc) updates object positions frame by frame, thus rendering continuously, and making the animation smooth through glutPostRedisplay().


Rendering & Display

The whole scene is rendered frame by frame using OpenGL primitives: GL_QUADS, GL_TRIANGLE_FAN, and GL_LINES. Ground, road, grass strips, and other decorative elements are added to make the scene more realistic. When combined with animation, color interpolation, and user interaction, the project offers a dynamic and aesthetically pleasing cityscape with smooth, real-time animations.


Output

The project output is a completely animated city scene visualized through OpenGL. The scene consists of various graphical elements like buildings, cars, trees, clouds, the sun/moon, and birds which are all arranged nicely to make an attractive layout. The animations are in real-time, and they are showing very smoothly such as the movement of cars with rotating wheels, birds flying with flapping wings, clouds moving across the sky, and trees gently swaying. A gradual transition from day to night is shown by changing the sky color and by the lighting of the buildings. User control is made easier with the help of interactive features like Night Mode and Pause/Resume. To sum up, the output presents a complete, animated, and organic city environment that is built by means of OpenGL transformations, animation logic, and rendering techniques. 

Discussion
The project effectively illustrates the use of OpenGL for developing an entire animated 2D city scene. The implementation emphasizes various fundamental concepts of graphics, such as the rendering of shapes, applying transformations, blending colors, and an object-based modeling approach. Through the implementation of GLUT's timer functionality, a smooth loop for frame updates is maintained, thus making the movement of the car, rotating wheels, drifting clouds, flying birds, and swaying trees consistent. The implementation and control of timing and user input are done effectively, enabling interactive control on the user's side via the pause and resume feature, thus providing better control for animating. The implementation of nighttime and automatic headlights functionality introduces realism into the scene and clearly illustrates the benefits of smooth transition effects on user experience. The project not only illustrates learning concepts within CSE422 but also effectively illustrates a learning- based approach, as various graphics concepts have been seamlessly brought together.
