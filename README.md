# Tufts Robotics Club Fall 2022 OpenCV Workshop

Example code used in the Tufts Robotics Club's Fall 2022 OpenCV Workshop, in preparation for the CVLSRS competition. A Google Colab notebook containing some of the code and an explanation of the OpenCV functions used in it can be found [here](https://colab.research.google.com/drive/1RezOkYKO5iILtLxFNHqnSSZKsGk3lOPv?usp=sharing).

## Dependencies

This code was written and tested on Python 3.9.10. Required packages (with versions) are listed in [requrements.txt](requrements.txt).

## How to Run

Since this code was written for a workshop geared toward all skill levels, this section will first describe how to set up a virtual environment and install requrements; a process that can be used in running virtually any Python program. For those with Python experience, who already know the general process for installing dependencies, skip to the "Running the Code" subsection.

### Setting Up a Virtual Environment

You can think of a virtual environment as an isolated python box on your computer, separate from your main python installation, where you can install whatever libraries and such that you want without breaking the dependencies on other projects. This is good practice to do with any Python project; in this tutorial we will be using venv, which isn’t the only way to do it, but it definitely the easiest to set up.

1. In the base directory for the project, run `python3 -m venv env`. This should create a directory called "env" in which the virtual environment will be stored.

2. Now run `. env/bin/activate` to activate the virtual environment. This should make any future Python commands run in this terminal window use the virtual environment, rather than your main Python installation. To ensure this is working correctly, you can run `which python3` and ensure the path given points to something inside that /env directoory created in the last step.

3. Next, use pip, Python's package manager, to install the dependencies by running `python3 -m pip install -r requrements.txt`. This command is essentially iterating through each line of requrements.txt and telling pip to install the package listed there.

### Running the Code

Once you have installed the appropriate dependencies, you should now be able to run the code!

To run the triangle recognition program on a static image: `python3 shape_recognition_example scan_static_image.py <path_to_image>`

To run the triangle recognition program on local webcam feed: `python3 shape_recognition_example scan_webcam_feed.py`
