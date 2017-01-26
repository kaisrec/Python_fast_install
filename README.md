***Installer Python et son environnement sur un PC***

I) <span style="text-decoration: underline;">Les logiciels indispensables</span>

Pour pouvoir travailler correctement et confortablement avec Python, il faut installer:  
    1) Obligatoire: une version de Python adaptée au système d'exploitation de l'ordinateur  
    2) Obligatoire: les bibliothèques  (ou librairies, ou packages) annexes nécessaires et adaptées à la version installée de Python  
    3) Facultatif: un EDI (Environnement de développement intégré) plus confortable sur IDLE (l'environnement par défaut) et compatible avec la version de Python

1) <span style="text-decoration: underline;">Installer Python</span>

  Vous trouverez sur le site officiel de <span>[<span class="HyperlinkInline">Python</span>](https://www.python.org/downloads/)</span> la dernière version de Python adaptée à l'OS de votre ordinateur. Avec Windows 64 bits, il faudra télécharger et exécuter le fichier disponible sous l'appellation "Windows x86-64 MSI installer". En mai 2015, ce fichier est  python-3.4.3.amd64.msi, correspondant à la dernière version de Python 3.4.  
Plusieurs versions de Python 3.3 et 3.4 par exemple peuvent cohabiter sans problèmes.

2) <span style="text-decoration: underline;">Installer avec pip les packages indispensables à un environnement de travail scientifique</span>

  Il y a quatre packages indispensables: numpy, scipy, matplotlib et pillow. Python intègre depuis la version 3.4 un outil de gestion des packages, pip (pour package installation python), dont l'exécutable est situé dans C:\Python34\Scripts.  
  En cas de besoin, consulter le <span>[<span class="HyperlinkInline">site officiel de pip</span>](https://pip.pypa.io/en/latest/index.html)</span>. Voilà comment l'utiliser avec un PC sous Windows et connecté à l'internet:

(1) Télécharger sur le site de <span>[<span class="HyperlinkInline">Christoph Gohlke</span>](http://www.lfd.uci.edu/~gohlke/pythonlibs/)</span>  (ou récupérer sur une clé usb) les fichiers .whl des packages désirés correspondant à la version de Python. Avec Python 3.4 et en mai 2015, ces fichiers s'appellent:  
    • numpy-1.9.2+mkl-cp34-none-win_amd64.whl  
    • scipy-0.15.1-cp34-none-win_amd64.whl  
    • Pillow-2.8.1-cp34-none-win_amd64.whl  
    • matplotlib-1.4.3-cp34-none-win_amd64.whl  
(2) Recopier ces fichiers dans le répertoire C:\Python34\Scripts  
(3) Créer un fichier batch (d'extension .bat) contenant les lignes suivantes, qui doivent être adaptées si les noms ont changés

cd C:\Python34\Scripts  
    pip install numpy-1.9.2+mkl-cp34-none-win_amd64.whl  
    pip install scipy-0.15.1-cp34-none-win_amd64.whl  
    pip install Pillow-2.8.1-cp34-none-win_amd64.whl  
    pip install matplotlib-1.4.3-cp34-none-win_amd64.whl  
pause

(4) Exécuter ce fichier batch: les packages sont installés. De plus d'autres petits packages nécessaires sont installés automatiquement (c'est pour cette raison que l'ordinateur doit être connecté pendant l'exécution du batch).  
  Si l'ordinateur n'est pas connecté à l'internet lors de l'exécution du batch, il faudra que votre batch contiennent les lignes suivantes et que les fichiers supplémentaires .whl aient été auparavant récupérés et recopiés dans le répertoire  C:\Python34\Scripts.

cd C:\Python34\Scripts  
    pip install numpy-1.9.2+mkl-cp34-none-win_amd64.whl  
    pip install scipy-0.15.1-cp34-none-win_amd64.whl
    pip install Pillow-2.8.1-cp34-none-win_amd64.whl 
    pip install pytz-2015.4-py2.py3-none-any.whl
    pip install pyparsing-2.0.3-py3-none-any.whl
    pip install python_dateutil-2.4.2-py2.py3-none-any.whl
    pip install six-1.9.0-py2.py3-none-any.whl
    pip install matplotlib-1.4.3-cp34-none-win_amd64.whl
pause

<div style="font-family:Helvetica; font-size:11px; width:100%; border:1px none #999999; border-top-style:solid; padding-top:2px; margin-top:20px;"><span style="color:#555555">© 2015 - Eric Obermeyer</span>     </div>"# Python_fast_install" 
