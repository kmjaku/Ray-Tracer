# Ray Tracer

<img align="center" src="saved_img/1.png" width="100%" />
<br />
<br />
<br />
<img align="center" src="saved_img/2.png" width="100%" />

This [Ray Tracer](https://en.wikipedia.org/wiki/Ray_tracing_(graphics)) was created as a school project

Ray tracing is a rendering technique using 3d vectors to reproduce the reality effect of lights on shapes such as Sphere, Cylinder, Cones and Planes

We added the torus and triangle as complex shapes.

This program used OpenCL for parallel programming to accelerate the movement and the rendering speed

Project created on pure C with SDL (SDL2 & SDL2_image), GTK+3 & OpenCL

## Getting Started

On of our main objective was to create a smooth and responsive ray tracer, to reduce the rendering calculation through movement the image is pixelated

The final render is calculated when movement stops

<img align="center" src="img/pixel_movement.gif" width="100%" />

Be sure to check out [Keyboard Shortcuts](#keyboard-shortcuts) to fully enjoy the experience

### Prerequisites

Please once install GTK+3, SDL2 and SDL2_image.

Send me a notification if you find compatibility issues

## Installing

Clone with :

```
git clone https://github.com/kmjaku/Ray-Tracer.git ~/RT
cd ~/RT
make
```

Launch RT like :

```
./rt
```

Now, a window named RT is running, select :

```
Click [Open]
then select the folder you've cloned
then select [Scene]
and chose a scene [example.rt]
```

Modify and play around with the scene files available in the Scene folder, you can even make your own !

Send me a notification if you find compatibility issues

### Clean

Clean your directory using the available commands

Delete object files

```
make clean
```

Delete binaries and libraries

```
make fclean
```

## Keyboard Shortcuts

The shortcut are essential to navigate in the scene and move objects

### Camera Controls

- <kbd>w</kbd> / <kbd>s</kbd> rotate camera up / down
- <kbd>a</kbd> / <kbd>d</kbd> rotate camera left / right
- <kbd>&uarr;</kbd> / <kbd>&darr;</kbd> move forward / backward
- <kbd>&larr;</kbd> / <kbd>&rarr;</kbd> move left / right
- <kbd>pageup</kbd> / <kbd>pagedown</kbd> move up / down
- <kbd>tab</kbd> reset to initial position

### Objects Controls

Select an object with `Left Click`. Unselect with `Right Click`

Object movement (arrows) and rotation (w/a/s/d) use the same controls as the camera

- <kbd>x</kbd> / <kbd>c</kbd> / <kbd>v</kbd> modify object color with r/g/b values
- <kbd>+</kbd> / <kbd>-</kbd> modify object size
- <kbd>f</kbd> change object texture (note that some textures are only available for specific object type e.g Sphere)
- <kbd>n</kbd> modify the intensity of normal variation for bump mapping
- <kbd>delete</kbd> delete object
- <kbd>z</kbd> print object informations on the terminal
- <kbd>i</kbd> add sphere (on current position)
- <kbd>u</kbd> add torus (on current position)
- <kbd>y</kbd> add plan (on current position)
- <kbd>t</kbd> add light (on current position)
- <kbd>r</kbd> add triangle (on current position)

### Options Controls

- <kbd>q</kbd> apply filter to the scene (sepia/negative/blue-saturated/grey/red/green/blue)
- <kbd>k</kbd> / <kbd>l</kbd> + / - antialiasing
- <kbd>o</kbd> save a render in `img/` folder
- <kbd>m</kbd> activate motion blur
- <kbd>n</kbd> increase bump mapping intensity (only on objects with bump mapping activated)
- <kbd>1</kbd> / <kbd>2</kbd> / <kbd>3</kbd> / <kbd>4</kbd> / <kbd>5</kbd> switch scene

## Frameworks used

* [SDL](https://www.libsdl.org/) - The graphic library
* [OpenCL](https://www.khronos.org/opencl/) - API for parallel programming
* [GTK](https://www.gtk.org) - is a cross-platform widget toolkit for creating graphical user interfaces.

## Contact & Copyright

Project done with Brahim EL BAZ, Ibrahima TRAORE & Thibaut CHIN
If you want to contact me, you can send me a mail at kmjaku@student.42.fr

### Acknowledgments

* My thanks to the [42](http://www.42.fr/) school where we worked countless hours to finish this project
