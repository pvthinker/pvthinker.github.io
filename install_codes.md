git clone Fluid2d and pyRSW. To copy-paste from your computer to the virtual desktop, use the copy-paste interactive window on the left

> git clone https://github.com/pvthinker/Fluid2d.git

> git clone https://github.com/pvthinker/pyRSW.git

create the conda environement (this step may fail in that case, execute the next step). It takes a few minutes to download everything. It’s a bit a shame to have to download all these packages in your $HOME but that’s how it works.

> cd Fluid2d

> conda create --name fluid2d --file requirements.txt

if conda create fails

> conda init bash

then close the terminal, reopen a new one, module load anaconda3 and repeat the conda

> create --name fluid2d --file requirements.txt

That should work.

activate this environment

> conda activate fluid2d

you can now build Fluid2d

> .install.sh

last step, make Python aware of where Fluid2d is

> source ~/.fluid2d/activate.sh

you’re good to run Fluid2d

Second time with pyRSW

repeat the steps up to and including

> conda activate fluid2d

complete this environement with

> conda install numba pyaml

now install pyRSW

> cd

> cd Codes/pyRSW

> ./install.sh

make Python aware and you’re good to run it

> source ~/.pyrsw/activate.sh

> cd myexp/dipole

> python3 dipole.py
