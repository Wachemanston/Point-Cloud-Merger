# Point Cloud Merger

## Usage
Merge the real point cloud with the augumented point cloud.

## Environment
* Ubuntu 18.04

## Requirement
* [PCL Library](https://pointclouds.org/).  Lastest version is good.

## How to Run
1. `cd` to the main directory.
2. `cmake -S . -B build`
3. `cmake --build build`
3. `./build/main </path/to/realdata> </path/to/augmentdata>`
4. The generated data will be saved at `./output`.
