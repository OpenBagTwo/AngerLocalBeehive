# AngerLocalBeehive
A repository of Minecraft-related Jupyter notebooks:
- exploring Minecraft data structures
- scripting tedious actions for resource / datapacks
- prototyping assorted projects

## Installation and Usage

The notebooks in this repo are intended to be viewed **in Github**, which has a built-in notebook renderer. As such, you'll be best
served treating this notebook as a reference of code examples and not as a repository of actual scripts or running code.

This repo contains no packages or modules, and any custom methods are defined as macros in the notebooks themselves.

### That being said...

The development environment for running these notebooks is provided as [a conda environment YAML](environment.yml), so
the easiest way to run the code in this repo will be to:

1. Install some conda distribution (I highly recommend [`mambaforge`](https://github.com/conda-forge/miniforge#mambaforge))
  and [make sure it's configured to pull packages from the conda-forge repository.](https://conda-forge.org/docs/user/introduction.html#how-can-i-install-packages-from-conda-forge)
  
1. Clone or download this repository.

1. Navigate to the project root and create the execution environment using:
   ```bash
   $ mamba env create
   ```
   (substituting `conda` for `mamba` if needed)
   
1. Activate the environment via
   ```bash
   $ mamba activate beehive
   ```
   (again, use `conda activate` if you're not using `mamba`)

1. Set the path to the world you're looking to explore via an environment variable named `SAVE_PATH`, _e.g._
   ```bash
   $ export SAVE_PATH="/home/openbagtwo/.minecraft/saves/New World"
   ```

1. Start Jupyter
   ```bash
   $ jupyter lab
   ```

## Contributing

This is my own personal notebook repository. If you have code feedback or suggestions,
I welcome them (feel free to [open an issue](../../issues/new)), but otherwise
I advise creating your own [forking](../../fork).

## License

All notebooks in this repository are licensed under GPLv3. If you have a use case for adapting this code that requires a more
permissive license, please post an issue, and I'd be more than willing to consider a dual license.
