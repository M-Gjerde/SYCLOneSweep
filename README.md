# SYCL Implementation of Nvidia's OneSweep

Welcome to the SYCL implementation of Nvidia's OneSweep! This project is an open-source, high-performance implementation designed to efficiently sort 1 billion 32-bit key/value pairs using Nvidia's RTX 4090 GPU.

## Highlights

- **Blazing Fast Performance**: Achieves sorting of 1 billion (2^30) 32-bit key/value pairs in just 0.17 seconds (5.88 GKeys/s) on Nvidia RTX 4090. (Slightly slower than cuda implementation, but optimizations can still be done)
- **Open Source**: Completely free to use and modify under the MIT license.
- **SYCL Compatibility**: Leverages SYCL for cross-platform compatibility and future-proofing.
- **Efficient Resource Usage**: Optimized to make the most of GPU resources without requiring proprietary CUDA libraries.

## Getting Started

### Prerequisites

- Nvidia RTX 4090 GPU (or other compatible GPUs)
- SYCL-compatible compiler (e.g., Intel DPC++, Codeplay ComputeCpp)
- CMake (for building the project)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/sycl-onesweep.git
   cd sycl-onesweep
   mkdir build
   cd build
   cmake ..
   make
   ./onesweep_sycl


## License
This project is licensed under the MIT License. See the LICENSE file for more details.


## Special Thanks
A special thanks to the b0nes164/OneSweep repository for providing a CUDA library-less implementation that inspired and facilitated this project. https://github.com/b0nes164/OneSweep