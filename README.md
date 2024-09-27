# pricingerror-bot
This Python script automates the task of checking and interacting with order-related data across multiple browser tabs. It uses the pyautogui library to handle mouse movements, clicks, and keyboard interactions.

Features

    •    Automates interaction with multiple tabs.
    •    Uses mouse clicks to interact with specific screen positions, such as clicking on a dot next to an order number.
    •    Includes a failsafe mechanism that allows you to stop the script by moving the mouse to a corner or pressing ‘q’.
    •    Simple, repetitive task automation to minimize manual errors in managing order data.

How it Works

    
The script opens and interacts with a specified number of browser tabs.
It clicks on specific positions on the screen, such as the dot next to the number in the site with the list of links.
To stop the script, press ‘q’ or move the mouse to a screen corner, which will trigger the pyautogui.FAILSAFE.

Installation

To run the script, ensure you have the following dependencies installed:

pip install pyautogui
pip install pywin32

Usage

    
Resize your browser to 80% and ensure you have the site with the list of links page open with the amount of tabs you want to open visible.
Hover over the first link.
Run the script in your Python environment.
The script will continue to interact with the tabs until it completes the task or is manually stopped.

Alternative Approach

An alternative way to achieve this automation would be to use the pyautogui.locateOnScreen() function to locate visual elements instead of using specific screen coordinates. However, I opted for a solution that checks colors at specific positions on the screen, which is faster and more efficient in this use case. Checking colors eliminates the need to process screenshots, thus reducing the overhead of image recognition.

However, depending on your screen resolution or other factors, color-checking might still provide a more reliable and faster solution.

Contribution

Feel free to contribute to this project by submitting a pull request or reporting issues on GitHub.

Let me know if you’d like any modifications or further information in the README!
