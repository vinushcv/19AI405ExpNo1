<h1>ExpNo 1 :Developing AI Agent with PEAS Description</h1>
<h3>Name: VINUSH.CV</h3>
<h3>Register Number: 212222230176</h3>

<h3>AIM:</h3>
<br>
<p>To find the PEAS description for the given AI problem and develop an AI agent.</p>
<br>
<h3>Theory</h3>
<h3>The Vacuum Cleaner Agent:</h3>
<p>
The Vacuum Cleaner Agent is a Python class that simulates the behavior of a basic vacuum cleaner in a two-location environment ("A" and "B"). The agent can perform four actions: move left, move right, suck dirt, and do nothing. Its state includes the current location and dirt status in each location. The agent's initial state is at location "A" with no dirt. Actions like moving and sucking dirt can change its state, and the print_status method displays the current location and dirt status. This agent provides a foundation for simple vacuum cleaner simulations and can be adapted for more complex scenarios</p>
<hr>
<h3>PEAS DESCRIPTION:</h3>
<table>
  <tr>
    <td><strong>Agent Type</strong></td>
    <td><strong>Performance</strong></td>
     <td><strong>Environment</strong></td>
    <td><strong>Actuators</strong></td>
    <td><strong>Sensors</strong></td>
  </tr>
    <tr>
    <td><strong>cleaning Dirt</strong></td>
    <td><strong>Rooms,floor</strong></td>
     <td><strong>Dirt,cleaning</strong></td>
    <td><strong>Medicine, Treatment</strong></td>
    <td><strong>Location,Sensing Dirt</strong></td>
  </tr>
</table>
<hr>
<H3>DESIGN STEPS</H3>
<h3>STEP 1: Identifying the input</h3>
<p>Location</p>

<h3>STEP 2:Identifying the output:</h3>
<p>move_left: Moves the agent to the left if it is currently at location "B.".</p>
<p>move_right: Moves the agent to the right if it is currently at location "A."</p>
<p>suck_dirt: Sucks dirt in the current location if there is dirt present.After sucking dirt, status in that location is updated to indicate cleanliness.</p>
<p>do_nothing: Represents a passive action where the agent remains idle.</p>

<h3>STEP 3: Developing the PEAS description:</h3>
  <p>PEAS description is developed by the performance, environment, actuators, and sensors in an agent.</p>

<h3>STEP 4: Implementing the AI agent:</h3>
 <p>Clean the room and Search for dirt and Suck it.</p>


## program:
```py
Developing AI Agent with PEAS Description
Developed by: VINUSH.CV
RegisterNumber: 212222230176

class VacuumCleanerAgent:
    def __init__(self):
        # Initialize the agent's state (location and dirt status)
        self.location = "A"  # Initial location (can be "A" or "B")
        self.dirt_status = {"A": False, "B": False}  # Initial dirt status (False means no dirt)

    def move_left(self):
        # Move the agent to the left if possible
        if self.location == "B":
            self.location = "A"

    def move_right(self):
        # Move the agent to the right if possible
        if self.location == "A":
            self.location = "B"

    def suck_dirt(self):
        # Suck dirt in the current location if there is dirt
        if self.dirt_status[self.location]:
            self.dirt_status[self.location] = False
            print(f"Sucked dirt in location {self.location}")

    def do_nothing(self):
        # Do nothing
        pass

    def perform_action(self, action):
        # Perform the specified action
        if action == "left":
            self.move_left()
        elif action == "right":
            self.move_right()
        elif action == "suck":
            self.suck_dirt()
        elif action == "nothing":
            self.do_nothing()
        else:
            print("Invalid action")

    def print_status(self):
        # Print the current status of the agent
        print(f"Location: {self.location}, Dirt Status: {self.dirt_status}")

# Example usage:
agent = VacuumCleanerAgent()


# Move the agent, suck dirt, and do nothing

agent.perform_action("left")
agent.print_status()
agent.perform_action("suck")
agent.print_status()
agent.perform_action("nothing")
agent.print_status()
```
## Output:
![WhatsApp Image 2024-09-25 at 10 26 20_351f38ac](https://github.com/user-attachments/assets/90cd8a71-3aeb-43f1-899b-2629d3075228)


## Result:
Thus the Developing AI Agent with PEAS Description was implemented using python programming.

