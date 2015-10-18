# Avoid_Conflicts_Installing_Edx_SparkVM

Following the instructions to setup a VM for the classes <a href="https://www.edx.org/course/introduction-big-data-apache-spark-uc-berkeleyx-cs100-1x">Introduction-Big-Data-Apache-Spark</a> & <a href="https://www.edx.org/course/scalable-machine-learning-uc-berkeleyx-cs190-1x">Scalable-Machine-Learning</a> 

1. Download <a href="https://www.vagrantup.com/downloads.html">Vagrant</a> 
2. Download <a href="https://www.virtualbox.org/wiki/Downloads">VirtualBox</a>  
Note: Do not install the latest version of VirtualBox because the VirtualBox provider is compatible with VirtualBox versions 4.0.x, 4.1.x, 4.2.x, 4.3.x, and 5.0.x
3. Unzip <a href="https://github.com/spark-mooc/mooc-setup">MOOC Spark-setup zipFile</a>
4. Create your vagrant file and inside it copy the Vagrantfile 
5. Change the settings of the Vagrant file because it tries to connect to an outdated box version 

master.vm.box = "sparkmooc/base2" --> master.vm.box = "sparkmooc/base2"

I made this change after wasting some hours to setup the VM and there is nowhere a reference about it.                   
6. Type the command vagrant up and the sparkvm after some minutes is setup                                              
7. Then the world is yours....SparkVM under JupyterNotebook is done!!!

