# Sind Blitze sind Donner
"Sind Blitze sind Donner" in Bach's St. Matthew Passion, arranged for Minecraft's noteblocks.

Recording: https://youtu.be/38oW2-jAk6k

## Arrangement
Noteblock's capabilities are quite limited, so lots of compromises had to be made.

Key: G-sharp minor (transposed up 4 semitones from original)

Tempo: quarter note = 150 bpm (about 25% slower than a typical performance)

Instrumentation:
* Basso continuo: bass
* Bass: guitar
* Tenor: iron xylophone
* Alto: bit
* Soprano: flute
* Viola, violin II, violin I: harp
* Flute, oboe II, oboe I: bell 

While I try to keep the voices as close to original as possible, lots of individual notes and passages in the orchestra are transposed up or down an octave to fit their instrument's range.

## Play requirement
Minecraft java 1.18+.

If your device supports it, turn on Directional Audio to enjoy the double orchestras & choruses in stereo.

## Easy install 
Copy the `World` folder into your saves. 

To obtain the folder, you may clone the repo or use third-party tools such as [Down-Git](https://minhaskamal.github.io/DownGit) to download it.

## Build from source
### Build requirements
* python 3.10+
* pip
* git (optional)

### Overview of the build process
The structure is *almost* auto-generated using [noteblock-generator](https://github.com/FelixFourcolor/noteblock-generator). The program takes `coro1.json` and `coro2.json` which define the composition, and generates the structure inside an existing Minecraft world.

### Step-by-step guide

1. Install `noteblock-generator`:
    ```
    pip install --upgrade noteblock-generator
    ```
    Configure your PATH so that `noteblock-generator` is executable on the command line.

2. Obtain `coro1.json` and `coro2.json`. You may clone the repo or download just those files.

3. Obtain a world in Minecraft java 1.18+. You may use an existing world or create a new one. 

    For maximum performance, create a new world in creative mode, peaceful difficulty, superflat type, and no generated structures.

4. If you are inside the world, exit it first. Then,

    Generate:
    ```
    noteblock-generator [path to coro1.json] [path to minecraft world] --clear -o + + -

    noteblock-generator [path to coro2.json] [path to minecraft world] --clear -o + + +
    ```

5. `noteblock-generator` is not capable of automatically handling double orchestras & choruses (yet), so this last step must be done manually.

    Connect the two structures with a single redstone wire, like this: ![screenshot](screenshot.png)

## License
Do whatever you want.
