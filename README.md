# Onegin
Implementation of the string library with lines sorting algorithms.  
First task in MIPT in the first year of education.

## Motivation
The idea is to understand how to work with text files, how to properly represent them.

## How is it done?
The program receives the famous novel by Alexander Sergeevich Pushkin "Eugene Onegin" as input and based on the user's settings (modes of [`lexicographical`](https://en.wikipedia.org/wiki/Lexicographic_order) line sorting) sorts lines and writes them to the output file.  
Also there is documentation generated with [`doxygen`](https://en.wikipedia.org/wiki/Doxygen).

## What are the modes of lexicographical sorting?
1. Compare lines without punctuation;  
2. Compare lines with punctuation;
3. Reversed lines comparison. Given two strings, we iterate from the end to the beginning of them and do lexicographical sorting;
4. Direct lines comparison. Given two strings, we iterate form the beginning to the end of them and do lexicographical sorting.

## Generating documentation
1. [`Install doxygen`](https://www.doxygen.nl/download.html);
2. Add `doxygen/bin` directory to the environmental variables;
3. Cd (change directory) to the location of the `Onegin` project;
4. Open `Doxyfile` in notepad and set `OUTPUT_DIRECTORY` to your directory where you want the documentation to be, `INPUT` to the `Onegin` directory path, `USE_MDFILE_AS_MAINPAGE` to the path of the `README.md` file path (e.g. <your_path>/README.md);
5. Open terminal in the location of `Onegin` project;
6. Run `doxygen` command in terminal;
7. Open `html` directory and run `index.html` file.

## Setting up
**Clone the repository**
```
git clone https://github.com/V13kv/Onegin;
cd Onegin
```

**Compiling**
```
make init;
make
```

## Running
```
./onegin.exe
```
