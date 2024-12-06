**Setup Instructions**

Clone the repo

    $ git clone https://github.com/llvm/llvm-project.git
    $ cd llvm-project
configure it using

    $ cmake -S llvm -B build -G Ninja -DCMAKE_BUILD_TYPE=RelWithDebInfo -DLLVM_ENABLE_PROJECTS="clang;lld" -DCMAKE_INSTALL_PREFIX=/home/riscv_sec/llvm-install/ -DLLVM_USE_LINKER=lld  -DLLVM_INSTALL_ASSERTIONS=ON  -DLLVM_TARGETS_TO_BUILD="RISCV"
 Build Using

    $ cmake --build build -j80

Make using

    $ cmake --install build
