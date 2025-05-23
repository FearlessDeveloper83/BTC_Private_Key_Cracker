BTC Private Key Cracker

This python tool is used to get private key of a BTC address from within a list of such addresses.


REQUIREMENTS:

LINUX:
sudo python3 -m pip install --upgrade pip && pip3 install bit bip32utils

WINDOWS:
pip install bit bip32utils


run python3 check3.py 


Example: 
check3.py -r btc.txt -o found_key.txt -t 2 (CPU)
check3.py -r btc.txt -o found_key.txt -t 128 --gpu (GPU, depending on how many CUDA cores you have)

-r: Input file containing BTC addresses to look for
-o: Output file path to save valid keys
-t: threads to use of the corresponding component (CPU or GPU)
