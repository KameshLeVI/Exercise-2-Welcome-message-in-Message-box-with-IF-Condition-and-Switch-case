# Exercise-2-Welcome-message-in-Message-box-with-IF-Condition-and-Switch-case

## Aim:

To create a UiPath automation process that takes the user's name as input and displays personalized welcome messages based on the input using a IF condition and Switch case activity.

## Equipment Required:

UiPath Studio (installed on a compatible system).
Computer with:
Minimum 4 GB RAM.
Minimum 2.0 GHz CPU.
Windows operating system.
.NET Framework 4.6.1 or later.

## Procedure:

### Start a New Process:

Open UiPath Studio and create a new process.<br>
Name the project UiPath Switch Case Example.<br>

### Add Input Dialog Activity:

In the Activities tab, search for Input Dialog.<br>
Drag and drop the Input Dialog activity onto the main window.<br>
Set the Title property as "Enter Your Name", and the Label as "Please enter your name:".<br>
Create a variable userName to store the input from the user and assign the result to it.<br>

### Add IF Condition:

In the Activities tab, search for the IF.<br>
Drag the IF activity onto the main window, below the Input Dialog activity.<br>
In the Condition field of the IF activity, type userName = "RAM" to check if the user input is "RAM".

### Configure the True Branch:

In the Then section (True branch) of the IF activity, drag a Message Box activity.<br>
Set the Message field to "Welcome Mr. Ramachandran".

### Configure the False Branch:

In the Else section (False branch) of the IF activity, add Switch activity.

### Add Switch Activity:

In the Activities tab, search for the Switch activity.<br>
Drag the Switch activity under the Input Dialog activity.<br>
In the Expression field of the Switch activity, set the value to userName.<br>
Set the TypeArgument to String to handle text-based cases.<br>

### Configure Switch Cases:

Add cases to the Switch activity to handle specific inputs:<br>
a. Case 1: "RAM"<br>

Add a case with the label "RAM".<br>
Drag a Message Box activity into this case.<br>
Set the Message property to "Welcome Mr. Ramachandran".<br>
b. Case 2: "John"<br>

Add a case labeled "John".<br>
Drag a Message Box activity into this case.<br>
Set the Message to "Welcome Mr. John Doe".<br>
c. Case 3: "Sara"<br>

Add a case labeled "Sara".<br>
Drag a Message Box activity into this case.<br>
Set the Message to "Welcome Ms. Sara Smith".<br>

### Configure Default Case:<br>

In the Default section of the Switch, drag a Message Box activity.<br>
Set the Message to "Welcome " + userName, so it displays the user’s name for any other input.<br>

### Save and Run:

Save the project by pressing CTRL+S.<br>
Click on Run from the top-right corner to execute the workflow.

## UiPath WorkFlow:
![image](https://github.com/user-attachments/assets/97818d17-6210-48b3-8869-a3d4466d76e2)
![image](https://github.com/user-attachments/assets/9025e414-e02b-4714-9cbe-1612e7afbe49)
![image](https://github.com/user-attachments/assets/7db25ce0-ab34-4543-9eae-27caf264973f)
![image](https://github.com/user-attachments/assets/b7c327ab-9fae-499a-82b1-6990b7746756)
![image](https://github.com/user-attachments/assets/bf841335-f747-4f56-ae3f-1424df685d61)
![image](https://github.com/user-attachments/assets/4003a251-b99b-4b49-9e8d-23fc7e2f7b33)


## Result:

When the input is "RAM", a message box will display: "Welcome Mr. Ramachandran".<br>
When the input is "John", a message box will display: "Welcome Mr. John Doe".<br>
When the input is "Sara", a message box will display: "Welcome Ms. Sara Smith".<br>
For any other input, the message box will display: "Welcome " followed by the entered name.<br>
This demonstrates how the Switch activity can be used in UiPath to handle multiple cases based on user input.
