CPU Scheduling Simulator
Introduction
The CPU Scheduling Simulator is an interactive GUI-based application that helps users visualize and analyze various CPU scheduling algorithms, including FCFS (First-Come-First-Serve), SJF (Shortest Job First), Round Robin (RR), and Priority Scheduling. The application is designed to aid learning and experimentation with these algorithms by allowing users to input process details and view the scheduling results, including Gantt charts and performance metrics.

Step-by-Step Instructions
1. Prerequisites
Before running the project, ensure that your system meets the following requirements:

Operating System: Windows, macOS, or Linux
Python Version: Python 3.9 or higher
Pip: Python’s package manager should be installed
Git: Installed for cloning the repository
Required Libraries: The application requires third-party Python libraries, which will be installed via requirements.txt.
2. Installing Git
If Git is not installed on your system, follow the steps below to install it:

Windows:

Download the Git installer from Git for Windows.
Run the installer and follow the setup instructions.
Verify installation by running the following command in a command prompt:
bash
Copy code
git --version
macOS:

Open a terminal.
Run the following command to install Git:
bash
Copy code
brew install git
Verify installation by running:
bash
Copy code
git --version
Linux:

Use your package manager to install Git. For example:
bash
Copy code
sudo apt install git
Verify installation by running:
bash
Copy code
git --version
3. Clone or Download the Repository
Open a terminal or command prompt.
Clone the repository from GitHub using the following command:
bash
Copy code
git clone https://github.com/MohammedAhmeduddin/CPU_Scheduler
Alternatively, download the repository as a ZIP file from the GitHub page and extract it to a directory of your choice.
Navigate to the project directory:
bash
Copy code
cd cpu_schuduler.py
4. Set Up a Virtual Environment
To isolate dependencies, create a Python virtual environment:

Create the virtual environment:
bash
Copy code
python -m venv venv
Activate the virtual environment:
Windows:
bash
Copy code
.\venv\Scripts\activate
macOS/Linux:
bash
Copy code
source venv/bin/activate
5. Install Dependencies
Install the required Python libraries using the requirements.txt file:

bash
Copy code
pip install -r requirements.txt
This will install all necessary libraries, such as:

Tkinter: For building the GUI.
Matplotlib: For generating Gantt charts.
Pytest: For running unit tests.
6. File Structure Explanation
Below is the project file structure with explanations for each file and folder:

graphql
Copy code
cpu_schuduler.py/
├── main.py                  # Entry point for the application.
├── requirements.txt         # File containing a list of required Python libraries.
├── README.txt               # Instructions for setting up and running the project.
├── src/                     # Source code directory.
│   ├── algorithms/          # Contains implementations of scheduling algorithms.
│   │   ├── fcfs.py          # First-Come-First-Serve implementation.
│   │   ├── sjf.py           # Shortest Job First implementation (preemptive and non-preemptive).
│   │   ├── rr.py            # Round Robin implementation.
│   │   ├── priority.py      # Priority Scheduling implementation.
│   ├── gui/
│       ├── app_ui.py        # GUI design and controls.
├── tests/                   # Directory containing test cases for the application.
│   ├── test_fcfs.py         # Tests for FCFS algorithm.
│   ├── test_sjf.py          # Tests for SJF algorithm.
│   ├── test_rr.py           # Tests for Round Robin algorithm.
│   ├── test_priority.py     # Tests for Priority Scheduling algorithm.
main.py: The main script to run the application.
requirements.txt: Ensures all dependencies are installed correctly.
src/algorithms/: Contains the implementation of CPU scheduling algorithms.
src/gui/app_ui.py: Handles the graphical interface for user interactions.
tests/: Includes unit tests to verify the correctness of scheduling algorithms.
7. Running the Application
To start the CPU Scheduling Simulator:

Ensure the virtual environment is activated.
Run the following command:
bash
Copy code
python main.py
The GUI window will appear, allowing you to interact with the application.
8. Using the Simulator
Input Process Details:

Enter the following details for each process:
Process Name (e.g., P1, P2)
Burst Time
Arrival Time
Priority (for priority scheduling)
Click "Add Process" to add the process to the list.
Select Scheduling Algorithm:

Choose a scheduling algorithm from the dropdown menu.
If using Round Robin, specify the time quantum.
Run Simulation:

Click "Run Simulation" to execute the selected algorithm.
The results will display:
Gantt chart visualization.
Table with waiting and turnaround times.
Metrics like average waiting and turnaround times.
Reset or Exit:

Click "Reset" to clear inputs and outputs for a new simulation.
Click "Exit" to close the application.
9. Running Tests
To verify the correctness of the algorithms, run the test cases:

Navigate to the project directory.
Run the following command:
bash
Copy code
pytest
Pytest will execute all test cases in the tests/ folder and display the results.

10. Troubleshooting
Python Not Recognized: Ensure Python is installed and added to your system's PATH.
Module Not Found: Run pip install -r requirements.txt to ensure all dependencies are installed.
Permission Issues: Run the terminal or command prompt as an administrator (Windows) or use sudo (Linux/macOS).
Pip Version Issue: Upgrade pip using:
bash
Copy code
python -m pip install --upgrade pip
11. Acknowledgments
This project was created by the following team members:

Mohammed Aslam (mm2954@njit.edu)
Kyle Kissinger (kck6@njit.edu)
Ahmeduddin Mohammed (am3837@njit.edu)
If you encounter any issues or have questions, please contact the team for assistance.