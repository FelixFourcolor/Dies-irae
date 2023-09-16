# Dies irae
"Dies irae" in Mozart's Requiem, arranged for Minecraft's noteblocks.

Recording: https://youtu.be/3exOZnZT0w0

Note: The structure shown in the YouTube video was made at commit [40b4078](https://github.com/FelixFourcolor/Dies-irae/commit/40b40787490af010d4dd98415a79fe3330039dc1). A few improvements have been made since then. You can revert to this commit if you want an exact replica of what was shown in the video.

## Arrangement
Instrumentation:
* Soprano: bit
* Alto: bit
* Tenor: guitar
* Bass: guitar
* Violin I & II, viola: harp
* Cello: guitar
* Basset horn I & II: flute
* Bassoon I: iron xylophone
* Bassoon II: didgeridoo
* Trumpet I & II: pling
* Timpani: bass + base drum

Tranposed down one semitone to better fit noteblock's ranges. However, a few notes still do not fit, then they are either transposed up/down an octave or played by a different instrument, depending on which sounds better to me.

## Play requirement
Minecraft java 1.18+

## Easy install 
Copy the [World](https://github.com/FelixFourcolor/Dies-irae/tree/master/World) folder into your saves.

To obtain the folder, you may clone the repo or use third-party tools such as [Down-Git](https://minhaskamal.github.io/DownGit) to download it.

## Build from source
### Build requirements
* python >= 3.10, < 3.12
* pip

### Overview of the build process
The structure is auto-generated using [noteblock-generator](https://github.com/FelixFourcolor/noteblock-generator). The program takes [src](https://github.com/FelixFourcolor/Dies-irae/tree/master/src) which defines the composition, and generates the structure inside an existing Minecraft world.

### Step-by-step guide

1. Install the lastest version of [noteblock-generator](https://github.com/FelixFourcolor/noteblock-generator):
    ```
    pip install --upgrade noteblock-generator
    ```
    Configure your PATH so that `noteblock-generator` is executable on the command line.

2. Obtain [src](https://github.com/FelixFourcolor/Dies-irae/tree/master/src). You may clone the repo or download just that folder.

3. Obtain a world in Minecraft java 1.18+. You may use your existing world or create a new one. 

4. If you are inside the world, exit it first. Then,
    ```
    noteblock-generator --clear [path to src] [path to minecraft world]
    ```

    (See [noteblock-generator](https://github.com/FelixFourcolor/noteblock-generator)'s documentation for explanation and more build options.)

## License
This project, including the uploaded YouTube video, is given to the public domain. No rights reserved.
