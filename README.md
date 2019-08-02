# minimal SDL + OpenGL boilerplate

Press `R`, `G`, or `B` to chnage color.

## building

Only tested on Linux. Eventually, I will setup some docker magic to make it work on other systems.

Install dependencies:

```
apt install cmake libsdl2-dev libsdl2-image-dev libxmu-dev libxi-dev libgl-dev libglew-dev g++
```

Build:

```
cmake .
make
```


