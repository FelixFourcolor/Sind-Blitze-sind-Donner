# Sind Blitze, sind Donner
"Sind Blitze, sind Donner" in Bach's St. Matthew Passion, arranged for Minecraft's noteblocks.

Recording: https://youtu.be/38oW2-jAk6k

Note: A few changes have been made since the release of the YouTube video. You can switch to the [YouTube branch](https://github.com/FelixFourcolor/Sind-Blitze-sind-Donner/tree/YouTube) for an exact replica of what was shown in the video. Otherwise, stay on the main branch for the latest version.

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

## Play requirements
Minecraft java 1.19+. 

Go to Music & Sounds setting, turn on Directional Audio and turn down Jukebox/Note Blocks sound level to 50% (otherwise it's too loud).

## Easy install 
Copy the [World](https://github.com/FelixFourcolor/Sind-Blitze-sind-Donner/tree/main/World) folder into your saves.

To obtain the folder, you may clone the repo or use third-party tools such as [Down-Git](https://minhaskamal.github.io/DownGit) to download it.

## Build from source
### Build requirements
* python 3.10+
* pip

### Overview of the build process
The structure is *almost* auto-generated using [noteblock-generator](https://github.com/FelixFourcolor/noteblock-generator). The program takes [coro1.json](https://github.com/FelixFourcolor/Sind-Blitze-sind-Donner/blob/main/coro1.json) and [coro2.json](https://github.com/FelixFourcolor/Sind-Blitze-sind-Donner/blob/main/coro2.json) which define the composition, and generates the structure inside an existing Minecraft world.

### Step-by-step guide

1. Install the lastest version of [noteblock-generator](https://github.com/FelixFourcolor/noteblock-generator):
    ```
    pip install --upgrade noteblock-generator
    ```
    Configure your PATH so that `noteblock-generator` is executable on the command line.

2. Obtain [coro1.json](https://github.com/FelixFourcolor/Sind-Blitze-sind-Donner/blob/main/coro1.json) and [coro2.json](https://github.com/FelixFourcolor/Sind-Blitze-sind-Donner/blob/main/coro2.json). You may clone the repo or download just those files.

3. Obtain a world in Minecraft java 1.19+. You may use your existing world or create a new one.

4. If you are inside the world, exit it first. Then,
    ```
    noteblock-generator [path to coro1.json] [path to minecraft world] --orientation + + -

    noteblock-generator [path to coro2.json] [path to minecraft world] --orientation + + +
    ```

    (See [noteblock-generator](https://github.com/FelixFourcolor/noteblock-generator)'s documentation for explanation and more build options.)

    Wait for the program to finish, then head inside.

5. The generator is not capable of automatically handling double orchestras (yet), so this last step must be done manually.

    Connect the two structures with a single redstone dust, like this: ![screenshot](screenshot.png)
