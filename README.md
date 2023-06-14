Ce repo contient un paquet ROS dans lequel il existe un modèle de main de robot décrit à l'aide de l'Urdf (format de description de robot unifié). 

Ce document décrit les étapes à suivre pour configurer et afficher le modèle dans votre environnement ROS.


Prérequis:

ROS (Robot Operating System) installé sur votre système
RVIZ

Instructions de configuration

Créez un espace de travail catkin :

$ mkdir -p ~/NOM DU WORKPSACE_ws/src

$ cd ~/NOM DU WORKPSACE_ws/src

Clonez ce repo dans le dossier src  de l'espace de travail catkin:

$ git clone https://github.com/AKH211/ROS_URDF

Accédez au dossier urdf :

$ cd ~/NOM DU WORKPSACE_ws/src/main_urdf/urdf

Sourcez la distribution ROS :

$ source /opt/ros/%YOUR_ROS_DISTRO%/setup.bash


Compilez le package et sourcez le fichier de configuration :

$ cd ~/NOM DU WORKPSACE_ws

$ catkin build

$ source devel/setup.bash

Lancez la visualisation du modèle URDF  dans (NOM DU WORKPSACE_ws/src/main_urdf/urdf) avec la commande:

$ roslaunch urdf_tutorial display.launch model:=main.urdf


