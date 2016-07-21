# Tesseract Example

A very basic Tesseract-OCR example with C++ Archive Network building.

## Building

Supported OS: Windows, Linux.

### Windows

Prerequisites:

1. Download git, cmake and add them to PATH
2. Download the latest CPPAN (https://cppan.org/) client from https://cppan.org/client/
3. Add cppan to PATH too.

```
git clone https://github.com/cppan/tesseract_example tesseract_example
cd tesseract_example
cppan
mkdir build && cd build
cmake ..
cmake --build . --config Release
```

### Linux

Prerequisites:

1. Install git, cmake, the latest CPPAN (https://cppan.org/) client from https://cppan.org/client/ (.deb or .rpm client for your system, gcc-5 ABI is required).
2. Run

```
git clone https://github.com/cppan/tesseract_example tesseract_example
cd tesseract_example
cppan
mkdir build && cd build
cmake ..
make -j4
```

## Testing

1. Download tesseract english data to `tessdata` dir near the `main` binary.
2. Copy test image `img/phototest.tif`
3. Run ``main phototest.tif``
