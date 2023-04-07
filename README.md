# acnn
A gui tool to simplify working with neural network for beginners

## Setup one time
./getPackages.sh

## Setup python virtual environment
sudo apt-get install python3-venv
python3 -m venv venv
. venv/bin/activate

python3 -m pip install PyQt5
python3 -m pip install PyQt5-sip
python3 -m pip install PyQtWebEngine
pip install fann2

## C API library
mkdir build
cd build
cmake ../FANN-2.2.0-Source/
make all
cd src/
export LD_LIBRARY_PATH=$(pwd)

## Example python run
cd labs/xor-lab/
python xor-lab.py
python xor-lab-test.py

