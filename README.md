## SystemVerilog Project: Musical Synthesis

This repository hosts a SystemVerilog project that implements a musical synthesis system. The project uses Quartus project files to create a piano-like instrument. The notes for the piano have already been synthesized, making the project ready to run from the start.

### Overview

The project generates waveforms for different types of signals, such as sinusoid, sawtooth, square, and custom waveforms from `.wav` files. The generated waveforms can be used to create a musical instrument like a piano.

### How it works

The main SystemVerilog file (`main.sv`) allows users to choose the type of waveform they want to generate. The options are:

1. Sinusoid
2. Sawtooth
3. Square
4. All of them
5. Convert my own `.wav` file to samples

Depending on the user's choice, the script generates the corresponding waveform(s) and saves them as `.txt` and `.png` files in the `output_files` directory.

### Usage

To use the project, follow these steps:

1. Clone the repository to your local machine.
2. Make sure you have Quartus installed.
3. Open the `main.sv` file in Quartus and follow the prompts to generate the desired waveform(s).
4. Use the generated waveform(s) in your Quartus project to create a musical instrument.

### Example

Here's an example of how to generate a sinusoid waveform with 4096 samples and a sample depth of 2 bytes:

```
$ quartus main.sv
Enter the number of the waveform you want to generate:
Sinusoid (1) Sawtooth (2) Square (3) All of them (4) Convert my own wav file to samples (5): 1
How many samples do you want in your wave table (recommend 4096, or some large power of 2): 4096
You will need a 12 bit counter to index into your wave table
Generated txt and png files of your waveforms to output_files directory
```

After running the script, you can find the generated waveform files in the `output_files` directory.

### Contributing

Feel free to contribute to this project by submitting pull requests or opening issues on GitHub. Your feedback and contributions are greatly appreciated!
