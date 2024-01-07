# Dies irae

"Dies irae" in Mozart's Requiem, arranged for Minecraft's noteblocks.

Recording: <https://youtu.be/3exOZnZT0w0>

Note: A few changes have been made since the release of the YouTube video. You can switch to the [YouTube branch](https://github.com/FelixFourcolor/Dies-irae/tree/YouTube) for an exact replica of what was shown in the video. Otherwise, stay on the main branch for the latest version.

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
* Alto, tenor, bass trombones (doubling alto, tenor, bass) are omitted

Tranposed down one semitone to better fit noteblock's ranges. However, a few notes still do not fit, then they are either transposed up/down an octave or played by a different instrument, depending on which sounds better to me.

## Play requirements

Minecraft Java 1.20 to play the pre-built world; 1.19+ if you build from source.

Optionally, go to Music & Sounds settings and turn down Master Volume to about 50% to 60%, otherwise it might be a bit too loud.

## Easy install

Copy the [World](https://github.com/FelixFourcolor/Dies-irae/tree/main/World) folder into your saves.

To obtain the folder, you may clone the repo or use third-party tools such as [Down-Git](https://minhaskamal.github.io/DownGit) to download it.

## Build from source

### Build requirements

* python 3.10-3.12
* pip

### Overview of the build process

The structure is auto-generated using [noteblock-generator](https://pypi.org/project/noteblock-generator/). The program takes [src](https://github.com/FelixFourcolor/Dies-irae/tree/main/src) which defines the composition, and generates the structure inside an existing Minecraft world.

### Step-by-step guide

1. Install the lastest version of [noteblock-generator](https://pypi.org/project/noteblock-generator/):

    ```sh
    pip install --upgrade noteblock-generator
    ```

    Configure your PATH so that `noteblock-generator` is executable on the command line.

2. Obtain [src](https://github.com/FelixFourcolor/Dies-irae/tree/main/src). You may clone the repo or download just that folder.

3. Obtain a world in Minecraft Java 1.19+. You may use your existing world or create a new one.

4. Run:

    ```sh
    noteblock-generator [path to src] [path to minecraft world]
    ```

    See [noteblock-generator](https://pypi.org/project/noteblock-generator/) for more build options.
