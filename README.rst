------------------------
doodle jump game 
------------------------

.. image:: https://user-images.githubusercontent.com/79650307/227780633-9eb0e835-50d6-4a2e-a601-bb3f7e3bb598.png
.. image:: https://user-images.githubusercontent.com/79650307/227780675-4730020d-a2e6-437f-a5b7-bbc7224aaaf5.png

.. contents:: :depth: 3



About
------
Simply lightweight game on pygame also work in docker.



Usage
--------

Common run
~~~~~~~~~~

1. Clone
"""""""""""" 
Clone this repo and change your current directory:

::

    git clone git@github.com:mb6ockatf/doodle_jump.git && cd doodle_jump


2. Start game:
""""""""""""""""

::
 
   python3 src/start.py


3. Additionally
""""""""""""""""
Insert your nickname in main menu to save the record.



Docker (stable for Unix)
~~~~~~~~~~~~~~~~~~~~~~~~~~

1. Clone
""""""""""
Clone this repo and change your current directory:

::

    git clone git@github.com:mb6ockatf/doodle_jump.git && cd doodle_jump


2. Build
""""""""""""""""""""""
Run docker build:

:: 

    docker built -t doodle-jump .


3. ``xhost``
""""""""""""""""""""""""""""""""""""""
Setting  ``xhost``  before launch

:: 

    xhost +local:


4. Run image
""""""""""""""
Run image the final command:

::

    sudo docker run -e DISPLAY=unix$DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix doodle-jump


Controls table
-------------------
         
+-----------------------+-------------------+
| Action                | Description       |
+=======================+===================+
| ``>`` ``d``           | move to the right |
+-----------------------+-------------------+
| ``<`` ``a``           | move to the left  |
+-----------------------+-------------------+
| ``space`` ``↑`` ``w`` | pause             |
+-----------------------+-------------------+
| ``escape``            | pause or exit     |
+-----------------------+-------------------+



.. raw:: html

 <div style="display:flex;">
     <img src='https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54'>
     <img src='https://img.shields.io/badge/sqlite-%2307405e.svg?style=for-the-badge&logo=sqlite&logoColor=black'>
     <img src='https://img.shields.io/github/license/mb6ockatf/doodle-jump.svg'>
     <img src='https://img.shields.io/github/last-commit/mb6ockatf/doodle-jump.svg'>
 </div>
