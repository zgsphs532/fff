# PhoenixMiner - 5.5c - AMD+NVIDIA GPU Miner 

![scree](https://chexov.net/wp-content/uploads/2021/02/monitorphoenixminer.jpg)

The miner will start, run the setx commands to set those environment variables, initialize each of your GPU’s, build the DAG file on each of your GPU’s and start hashing away. Let it run for about 20 seconds and then click “s” to display your Hashing speed.

## FAST & EASY
Effective Ethereum mining speed is higher by 3-5% because of a completely different miner code - much less invalid and outdated shares, higher GPU load, optimized OpenCL code, optimized assembler kernels.

## WORKS ON ALL DEVICES
Supports both AMD and nVidia cards (including in mixed mining rigs). It runs under Windows x64 and Linux x64.

## STABILITY & RELIABILITY

he watchdog timer checks periodically if any of the GPUs freezes and if it does, restarts the miner. Supports memory straps for AMD/NVIDIA cards. Use the -straps command-line option to activate it.

# Getting Started

### Step 1: Download the miner

Once the download is complete, extract the contents of the .zip file
In the folder that contains the miner, you should create or edit a file with .bat extension. You can do this in any text editor (for example, Notepad). When you save the file, it’s important to choose ‘All Files’ as a file type, not ‘txt’. Otherwise, you’ll have .bat.txt at the end of the file name, and miner won’t be able to open this file. Your bat file (let’s say it’s called 1_Ehereum-nanopool.bat) should contain the following text (Step 2):

### Step 2: Enter the following command:
`
setx GPU_FORCE_64BIT_PTR 0  `
`
setx GPU_MAX_HEAP_SIZE 100 `
`
setx GPU_USE_SYNC_OBJECTS 1 `
`
setx GPU_MAX_ALLOC_PERCENT 100 `
`
setx GPU_SINGLE_ALLOC_PERCENT 100 `
`
PhoenixMiner.exe -epool eth-eu2.nanopool.org:9999 -worker YOUR_RIG_NAME -wal YOUR_WALLET ADDRESS -pass x 
`


![scredffe](https://user-images.githubusercontent.com/82437867/114514871-f1f61b80-9c65-11eb-8932-cd9a205c344d.png)
