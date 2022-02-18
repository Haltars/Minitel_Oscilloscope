# Minitel_Oscilloscope
Minitel Video/Audio Oscilloscope

Minitel + Entrée Video Composite + RaspberryPi + PureData 

ATTENTION!
L'ecran du Minitel est un tube cathodique qui contient de l'electricité statique, on peut donc en mourir si on met les doigts n'importe où et meme si il est débranché. Il faut donc le decharger pour ne pas prendre de risque. voir lien  https://www.youtube.com/watch?v=ZVXgdupoK54

Ensuite il faut rajouter une carte de conversion video pour pouvoir y brancher la sortie composite du RaspberryPi
Voir http://www.cfp-radio.com/realisations/rea48/minitel-01.html

Et modifier le fichier config.txt dans le dossier /boot de la carte sd pour configurer la sortie video.

Argumenter la ligne:

hdmi_force_hotplug=1

Desargumenter la ligne:

sdtv_mode=2

Ajouter les lignes:

sdtv_aspect=1
sdtv_disable_colourburst=1
overscan_left=45
overscan_right=40
overscan_top=0
overscan_bottom=0
