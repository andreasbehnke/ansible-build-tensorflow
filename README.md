# Install Tensor Flow
Installs tensor flow, based on this instruction:
https://www.tensorflow.org/install/install_linux#InstallingVirtualenv

== Specification ==

* installs CPU based implementation
* for ubuntu or ubuntu based systems
* phyton 3

== Install using method "virtualenv" ==
Using phyton virtual environment

* configure variables:
  * tensorflow_virtualenv_target_path defaults to ~/tensorflow
* ansible-playbook tensorflow_virtualenv.yml -l localhost --ask-sudo

Usage:

* source ~/tensorflow/bin/activate
* now you can use the tensorflow library
* type "deactivate" to leave virtualenv
* source code is checked out into folder ~/src/tensorflow using the branch which is
  compatible with the installed tensorflow version

== Install using method "build from sources" ==
 DO TO BE DONE
