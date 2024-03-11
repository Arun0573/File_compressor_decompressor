### title: Huffman Coding Decompressor and Compressor ###

### Decompression:

Reads the compressed file.

Extracts the embedded code table used for compression.

Iterates through the compressed data using the code table to reconstruct the original data byte by byte.

Writes the decompressed data to the output file

### Compression:

Reads the input file.

Analyzes the frequency of each character (symbol) to build a probability distribution.

Constructs a Huffman tree based on the symbol probabilities.

Assigns codewords (sequences of 0s and 1s) to each symbol based on the tree structure (shorter codewords for more frequent symbols).

Generates a code table that maps symbols to their corresponding codewords.

Iterates through the input file again, replacing each symbol with its codeword.

Writes the compressed data (containing codewords) and the code table to the output file.
