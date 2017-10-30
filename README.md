# Install Tensor Flow
Installs tensor flow, based on this instruction:
https://www.tensorflow.org/install/install_linux#InstallingVirtualenv

Specification:

* installs CPU based implementation
* using phyton virtual environment
* for ubuntu or ubuntu based systems
* phyton 3

Install:

* configure variables:
  * tensorflow_virtualenv_target_path defaults to ~/tensorflow
  * tensorflow_source_path defaults to ~/src/tensorflow
* ansible-playbook tensorflow -l localhost --ask-sudo

Usage:

* source ~/tensorflow/bin/activate
* now you can use the tensorflow library
* type "deactivate" to leave virtualenv
* source code is checked out into folder ~/src/tensorflow using the branch which is
  compatible with the installed tensorflow version
