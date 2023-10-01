# Sind Blitze, sind Donner
"Sind Blitze, sind Donner" in Bach's St. Matthew Passion, arranged for Minecraft's noteblocks.

Recording: https://youtu.be/38oW2-jAk6k

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

Go to Music & Sounds settings and turn on Directional Audio. Optionally, turn down Master Volume to about 60% to 70%, otherwise it might be a bit too loud (but of course this depends on your speakers).

## Easy install 
Copy the [World](https://github.com/FelixFourcolor/Sind-Blitze-sind-Donner/tree/YouTube/World) folder into your saves.

To obtain the folder, you may clone the repo or use third-party tools such as [Down-Git](https://minhaskamal.github.io/DownGit) to download it.

## Build from source
### Build requirements
* python >= 3.10, < 3.12
* pip

### Overview of the build process
The structure is *almost* auto-generated using [noteblock-generator](https://pypi.org/project/noteblock-generator/0.1.2.1/). The program takes [coro1.json](https://github.com/FelixFourcolor/Sind-Blitze-sind-Donner/blob/YouTube/coro1.json) and [coro2.json](https://github.com/FelixFourcolor/Sind-Blitze-sind-Donner/blob/YouTube/coro2.json) which define the composition, and generates the structure inside an existing Minecraft world.

### Step-by-step guide

1. Install [noteblock-generator 0.1.2.1](https://pypi.org/project/noteblock-generator/0.1.2.1/):
    ```
    pip install noteblock-generator==0.1.2.1
    ```
    Configure your PATH so that `noteblock-generator` is executable on the command line.

2. Obtain [coro1.json](https://github.com/FelixFourcolor/Sind-Blitze-sind-Donner/blob/YouTube/coro1.json) and [coro2.json](https://github.com/FelixFourcolor/Sind-Blitze-sind-Donner/blob/YouTube/coro2.json). You may clone the repo or download just those files.

3. Obtain a world in Minecraft java 1.19+. You may use your existing world or create a new one.

4. If you are inside the world, exit it first. Then,
    ```
    noteblock-generator --clear [path to coro1.json] [path to minecraft world] --orientation + + -

    noteblock-generator --clear [path to coro2.json] [path to minecraft world] --orientation + + +
    ```

    (See [noteblock-generator](https://pypi.org/project/noteblock-generator/0.1.2.1/)'s documentation for explanation and more build options.)

    Wait for the program to finish, then head inside.

5. The generator is not capable of automatically handling double orchestras (yet), so this last step must be done manually.

    Connect the two structures with a single redstone dust, like this: ![screenshot](screenshot.png)

## License
While Minecraft remains Mojang's property and is subjected to their terms of service, the source code used to generate this structure is given to the public domain. You are free to do whatever you want with it, as long as it complies with Minecraft's terms of service, without any restrictions from my end.

See [LICENSE](https://github.com/FelixFourcolor/Sind-Blitze-sind-Donner/blob/YouTube/LICENSE) for more details. 