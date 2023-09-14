# Sind Blitze, sind Donner
"Sind Blitze, sind Donner" in Bach's St. Matthew Passion, arranged for Minecraft's noteblocks.

Recording: https://youtu.be/38oW2-jAk6k

Note: The structure shown in the YouTube video was made at commit [e08cba0](https://github.com/FelixFourcolor/Sind-Blitze-sind-Donner/tree/e08cba0fd2dee93d267b618ae4f70846e8c5f646). A few improvements have been made since then. You can revert to this commit if you want an exact replica of what was shown in the video.

## Arrangement
Instrumentation:
* Soprano: flute
* Alto: bit
* Tenor: iron xylophone
* Bass: guitar
* Oboe I, oboe II, flute: bell
* Violin I, violin II, viola: harp
* Continuo: bass

Transposed up 4 semitones to better fit noteblock's ranges. However, a few notes still do not fit, then they are either transposed up/down an octave or played by a different instrument, depending on which sounds better to me.

## Play requirement
Minecraft java 1.18+

## Easy install 
Copy the [World](https://github.com/FelixFourcolor/Sind-Blitze-sind-Donner/tree/master/World) folder into your saves.

To obtain the folder, you may clone the repo or use third-party tools such as [Down-Git](https://minhaskamal.github.io/DownGit) to download it.

## Build from source
Note: The structure shown in the YouTube video was generated using [noteblock-generator 0.1.2.1](https://pypi.org/project/noteblock-generator/0.1.2.1/). Besides reverting to commit [e08cba0](https://github.com/FelixFourcolor/Sind-Blitze-sind-Donner/tree/e08cba0fd2dee93d267b618ae4f70846e8c5f646), you must also install this version to get an exact replica of what was shown in the video.

### Build requirements
* python 3.10+
* pip

### Overview of the build process
The structure is *almost* auto-generated using [noteblock-generator](https://github.com/FelixFourcolor/noteblock-generator). The program takes [coro1.json](https://github.com/FelixFourcolor/Sind-Blitze-sind-Donner/blob/master/coro1.json) and [coro2.json](https://github.com/FelixFourcolor/Sind-Blitze-sind-Donner/blob/master/coro2.json) which define the composition, and generates the structure inside an existing Minecraft world.

### Step-by-step guide

1. Install the lastest version of [noteblock-generator](https://github.com/FelixFourcolor/noteblock-generator):
    ```
    pip install --upgrade noteblock-generator
    ```
    Configure your PATH so that `noteblock-generator` is executable on the command line.

2. Obtain [coro1.json](https://github.com/FelixFourcolor/Sind-Blitze-sind-Donner/blob/master/coro1.json) and [coro2.json](https://github.com/FelixFourcolor/Sind-Blitze-sind-Donner/blob/master/coro2.json). You may clone the repo or download just those files.

3. Obtain a world in Minecraft java 1.18+. You may use your existing world or create a new one. 

4. If you are inside the world, exit it first. Then,
    ```
    noteblock-generator --clear [path to coro1.json] [path to minecraft world] --orientation + + -

    noteblock-generator --clear [path to coro2.json] [path to minecraft world] --orientation + + +
    ```

    (See [noteblock-generator](https://github.com/FelixFourcolor/noteblock-generator)'s documentation for explanation and more build options.)

    Wait for the program to finish, then head inside.

5. `noteblock-generator` is not capable of automatically handling double orchestras (yet), so this last step must be done manually.

    Connect the two structures with a single redstone dust, like this: ![screenshot](screenshot.png)

## License
This project, including the uploaded YouTube video, is given to the public domain. No rights reserved.
