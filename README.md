# BREAKtheGrid
Break out of the black box and allow users to show their creativity while increasing productivity. This hybrid work solution will make collaboration easier, more accessible, and much more enjoyable.

# Zoom Engage
<p align="center">
<img width="811" alt="Screen Shot 2023-02-18 at 10 49 18 PM" src="https://user-images.githubusercontent.com/66803124/219945596-73c3faa6-d330-484a-b551-379822832c4d.png">



Engage busts out of the black square grid and allows the user to show their creativity while increasing productivity. Engage will make collaboration easier, more effective, and much more enjoyable.



As a remote worker, I am constantly thinking of ways to improve video conferencing. 

The large black boxes on my screen all day have always felt uninspiring. Seeing online classrooms is even more jarring. In school, the teachers would always decorate their rooms with so much color and vibrance. Where is that vibrance now? 

With Zoom Engage, I wanted to bring it back. In doing so, Zoom can leverage the preference shown to its platform to pull ahead in market share.

<img width="480" alt="Screen Shot 2023-02-16 at 6 41 09 PM" src="https://user-images.githubusercontent.com/66803124/219512750-093f8197-0b8d-4f12-8249-a4cf22a2b0ac.png">

SO many companies are trying to compete in the video conferencing arena. But they all use the same uninspired black boxes. 

<img width="733" alt="Screen Shot 2023-02-16 at 6 48 37 PM" src="https://user-images.githubusercontent.com/66803124/219513706-23a7be51-03ed-44fd-b39f-77054cdf803d.png">

##### What if we broke away from this? <br>
##### What if we let the user decide what their work environment or classroom would look like? <br>
##### How much more creativity and productivity could we generate? <br>
##### How much much more preference for the Zoom platform could we foster? <br>
#### I am ready to find out. <br>

# Introducing BREAK the Grid

<img width="480" alt="Screen Shot 2023-02-16 at 5 29 50 PM" src="https://user-images.githubusercontent.com/66803124/219513853-ebe698be-e923-44fc-a08f-819d10536a14.png">

<img width="482" alt="Screen Shot 2023-02-16 at 5 29 32 PM" src="https://user-images.githubusercontent.com/66803124/219513866-2800e45a-1759-41e4-87f6-18f21ce45a93.png">

## For a new remote environments, whether that is at work, in the classroom, or catching up with friends, everyone deserves a place where they can feel like themselves and express their creativity. Not be boxed in. 

<img width="477" alt="Screen Shot 2023-02-16 at 5 30 18 PM" src="https://user-images.githubusercontent.com/66803124/219513885-73e25556-6297-49ee-9d14-f6d77818553a.png">


<img width="481" alt="Screen Shot 2023-02-16 at 5 30 32 PM" src="https://user-images.githubusercontent.com/66803124/219513900-ea32c2a7-6612-4c60-9c7a-b9892f85c549.png">


<img width="750" alt="Screen Shot 2023-02-16 at 8 23 22 PM" src="https://user-images.githubusercontent.com/66803124/219525615-2735fc31-edef-4c9b-8fea-b7469843353c.png">
</center>
Zoom API: The Zoom API (Application Programming Interface) is a set of rules and protocols that allows software applications to interact with the Zoom platform. This solution uses the Zoom API to retrieve the list of participants and their current status (mic on/off, video on/off, screen sharing on/off).

Zoom video SDK: Another option for creating a custom video conferencing solution with Zoom is to use the Zoom video SDK (Software Development Kit). The video SDK provides more control over the video conferencing experience and allows for the creation of custom interfaces and features.

Programming languages: This solution requires a programming language to implement the logic for calculating participant priorities, determining box sizes, and adjusting box sizes based on user input. The choice of programming language would depend on the platform and tools being used to develop the solution. Languages that interact with the Zoom API include Python, Java, and JavaScript. I chose Python for this implementation since it is the langauage I have the most experience in. 

User interface: This solution involves creating a custom user interface that allows the user to resize the boxes of the participants in a Zoom call.

Web technologies: It would likely involve the use of web technologies such as HTML, CSS, and JavaScript to create the user interface and handle user input.

### To create color selector GUI for the ZOOM grid using Tkinter:
1. Import the necessary modules: tkinter for creating the GUI, and askcolor from tkinter.colorchooser for opening a color selection dialog.
2. Define a Grid class that represents a grid of buttons, with methods for setting and getting the color of each button.
3. In the __init__ method of the Grid class, initialize the grid with the specified number of rows and columns, and set the colors of all buttons to white.
4. Define a GridGUI class that represents the GUI for the grid of buttons, with methods for handling button clicks and the color picker dialog.
5. In the __init__ method of the GridGUI class:
6. Create a new Grid object with the specified number of rows and columns.
7. Create a new tkinter window (self.root).
8. Create a 2D list of tkinter buttons, one for each button in the grid, and add them to the window. Each button is configured to call the on_button_click method with its row and column as arguments when it is clicked.
9. Create a tkinter button for opening the color selection dialog (self.color_picker_button), and add it to the window. When this button is clicked, it calls the on_color_picker_click method.
10. In the on_button_click method of the GridGUI class:
11. Get the current color of the button that was clicked using the Grid object's get_color method.
12. Toggle the color of the button between black and white.
13. Set the new color of the button using the Grid object's set_color method.
14. Update the background color of the button using the tkinter configure method.
15. In the on_color_picker_click method of the GridGUI class:
16. Open a color selection dialog using the askcolor method, and get the selected color.
17. Set the color of all buttons in the grid using the Grid object's set_color method.
18. Update the background color of all buttons in the grid using the tkinter configure method.
19. Define a run method in the GridGUI class that starts the tkinter main loop to display the window.
20. Create a new GridGUI object with the specified number of rows and columns.
21. Run the GUI using the run method of the GridGUI object.

### To create the Grid Resizing Solution:

Get the list of participants in the Zoom call using the Zoom API. This is necessary to determine the status of each participant (mic on/off, video on/off, screen sharing on/off), which is used to calculate participant priorities.

Calculate participant priorities based on their status, as follows:

Participants with screen sharing on have the highest priority.
Participants with both mic and video on have the second-highest priority.
Participants with mic on and video off have the third-highest priority.
Participants with mic off and video on have the fourth-highest priority.
Participants with both mic and video off have the lowest priority.
This prioritization ensures that participants who are actively contributing to the call (e.g. by screen sharing or having their video and mic on) are given more screen real estate.

Set the default box sizes based on participant priorities. The largest box will be allocated to the participant with the highest priority (screen sharing on), and the remaining boxes will be allocated in descending order of priority.

Create a custom user interface that allows the user to resize the boxes of the participants. This could be done using HTML, CSS, and JavaScript but will depend on the exact specifications of Zoom's environment. 

Implement logic to adjust the box sizes based on user input. When the user resizes a box, the size of the adjacent boxes should be adjusted to maintain the overall layout of the call.

Test the solution to ensure that it works as intended. This may involve testing with a variety of different call scenarios (e.g. different numbers of participants, different status combinations) to ensure that the box sizes are allocated correctly and can be resized by the user.

Deploy the solution to a web server or cloud platform so that it can be accessed by users. This could be done using services like AWS Elastic Beanstalk since Zoom is already integrated into the AWS Cloud. 

##### Coding steps are as follows:
1. Retrieve the list of participants and their current status (mic on/off, video on/off, screen sharing on/off) from the Zoom API.
2. Calculate the priority for each participant based on their status, following the order given in the prompt (screen share > mic+camera on > mic on > camera on > mic+camera off).
3. Sort the list of participants based on their priority, from highest to lowest.
4. Determine the desired size of each box for each participant, based on their priority. For example, the largest screen share participant might get 2/3 of the screen, while the smallest mic+camera off participant might get 1/6 of the screen.
5. Allow the user to change the size of each box individually by dragging its borders. As the user changes the size of a box, adjust the size of the other boxes accordingly to maintain the desired proportions.
6. If the user does not manually resize any boxes, display the boxes with the predetermined sizes based on their priority.


Information used to better understand ZOOM came from their community page and blog. 
https://support.zoom.us/hc/en-us/articles/201362323-Adjusting-your-video-layout-during-a-virtual-meeting





