# Sind Blitze, sind Donner
"Sind Blitze, sind Donner" in Bach's St. Matthew Passion, arranged for Minecraft's noteblocks.

Recording: https://youtu.be/oeLPMQ-b7cQ

## Arrangement
Instrumentation:
* Soprano: flute
* Alto: bit
* Tenor: iron xylophone
* Bass: guitar
* Flute I & II: bell 
* Oboe I & II: flute
* Violin I & II, viola: harp
* Cello: bass

Transposed up 4 semitones to better fit noteblock's ranges. However, a few notes still do not fit, then they are either transposed up/down an octave or played by a different instrument, depending on which sounds better to me.

## Play requirements
Minecraft java 1.19+. 

Go to Music & Sounds settings and turn on Directional Audio. Optionally, turn down Master Volume to about 50% to 60%, otherwise it might be a bit too loud (but of course this depends on your speakers).

Listening on headphones (or good stereo speakers) is strongly recommdended to fully enjoy the double orchestra.

## Easy install 
Copy the [World](https://github.com/FelixFourcolor/Sind-Blitze-sind-Donner/tree/main/World) folder into your saves.

To obtain the folder, you may clone the repo or use third-party tools such as [Down-Git](https://minhaskamal.github.io/DownGit) to download it.

## Build from source
### Build requirements
* python 3.10+
* pip

### Overview of the build process
The structure is auto-generated using [noteblock-generator](https://pypi.org/project/noteblock-generator/). The program takes [src](https://github.com/FelixFourcolor/Sind-Blitze-sind-Donner/tree/main/src) which defines the composition, and generates the structure inside an existing Minecraft world.

### Step-by-step guide

1. Install the lastest version of [noteblock-generator](https://pypi.org/project/noteblock-generator/):
    ```
    pip install --upgrade noteblock-generator
    ```
    Configure your PATH so that `noteblock-generator` is executable on the command line.

2. Obtain [src](https://github.com/FelixFourcolor/Sind-Blitze-sind-Donner/tree/main/src). You may clone the repo or download just that folder.

3. Obtain a world in Minecraft java 1.19+. You may use your existing world or create a new one.

4. If you are inside the world, exit it first. Then,
    ```
    noteblock-generator [path to src] [path to minecraft world]
    ```

    See [noteblock-generator](https://pypi.org/project/noteblock-generator/)for explanation and more build options.

    Warning: The pre-built [World](https://github.com/FelixFourcolor/Sind-Blitze-sind-Donner/tree/main/World) was generated using a modified version of noteblock-generator that allows the double orchestra to use two different themes. This feature is not ready to be published yet, so for now you can only choose one theme for the entire structure.

## License
While Minecraft remains Mojang's property and is subjected to their terms of service, the source code used to generate this structure is given to the public domain. You are free use it however you want, as long as such usage complies with Minecraft's terms of service, without any restrictions from my end.

See [LICENSE](https://github.com/FelixFourcolor/Sind-Blitze-sind-Donner/blob/main/LICENSE) for more details.