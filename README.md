# Install Tensor Flow
Installs tensor flow, based on this instruction:
https://www.tensorflow.org/install/install_linux

### Specification

* installs CPU based implementation
* for ubuntu or ubuntu based systems
* phyton 3

### Install using method "virtualenv"

Installing tensorflow using phyton virtual environment:

https://www.tensorflow.org/install/install_linux#InstallingVirtualenv

* configure variables:
  * tensorflow_source_path defaults to ~/src/tensorflow
  * tensorflow_virtualenv_target_path defaults to ~/tensorflow
* ansible-playbook tensorflow-virtualenv.yml -l localhost --ask-sudo

Usage:

* source ~/tensorflow/bin/activate
* now you can use the tensorflow library
* type "deactivate" to leave virtualenv
* source code is checked out into folder ~/src/tensorflow using the branch which is
  compatible with the installed tensorflow version

### Install using method "build from sources"

Build tensorflow PIP package from tensorflow sources:

* configure variables:
  * tensorflow_source_path defaults to ~/src/tensorflow
* ansible-playbook tensorflow-build.yml -l localhost --ask-sudo
* cd ~/src/tensorflow
* ./configure
* bazel build --config=opt //tensorflow/tools/pip_package:build_pip_package
* bazel-bin/tensorflow/tools/pip_package/build_pip_package /tmp/tensorflow_pkg
* sudo pip3 install /tmp/tensorflow_pkg/tensorflow-1.4.0rc1-cp35-cp35m-linux_x86_64.whl
