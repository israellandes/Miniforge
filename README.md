# Miniforge
[How to install Conda on Le Potato Ubuntu Versions?](https://hub.libre.computer/t/how-to-install-conda-on-le-potato-ubuntu-versions/1516)

---
# Failed Test

## When I try to run the installer:

wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-aarch64.sh

bash Miniconda3-latest-Linux-aarch64.sh
I get this error:

Miniconda3-latest-Linux-aarch64.sh: line 358: 25417 Illegal instruction (core dumped) “$CONDA_EXEC” constructor --prefix “$PREFIX” --extract-conda-pkgs

It works on other VPS like Amazon ec2s , how can I get a conda environment installed on my Le Potato?

PS. I also tried installing Anaconda as an alternative, but this process got hung up on the command line.

---
# Solution

## Use Miniforge if your trying to install Conda environment on Le Potato or Raspberry Pi like computers.

`wget https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-Linux-aarch64.sh`<br>
`sha256sum Miniforge3-Linux-aarch64.sh`<br>
`chmod +x Miniforge3-Linux-aarch64.sh`<br>
`./Miniforge3-Linux-aarch64.sh`<br>
`# Exit & Re-enter shell`<br>
`conda activate base`<br>
<br>
Cheers.
