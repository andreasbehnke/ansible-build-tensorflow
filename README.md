# Install Tensor Flow
Installs tensor flow, based on this instruction:
https://www.tensorflow.org/install/install_linux#InstallingVirtualenv

Specification:

* installs CPU based implementation
* using phyton virtual environment
* for ubuntu or ubuntu based systems
* phyton 3

Install:

* ansible-playbook tensorflow -l localhost --ask-sudo

Usage:

* source ~/tensorflow/bin/activate
* now you can use the tensorflow library
* type "deactivate" to leave virtualenv
