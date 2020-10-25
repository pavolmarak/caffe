# Caffe
Manjaro setup:

1. Clone the repo.
1. Run cmake-gui
1. Configure (pouzit systemovy kompilator gcc)
1. Install dependencies.
1. Install [CUDA 10.2](https://developer.nvidia.com/cuda-10.2-download-archive) (ak sa CUDA instaluje pomocou .run suboru, treba pri spusteni prikazu pouzit prepinac --override, aby sa ignorovalo hlasenie o GCC nekompatibilite)
1. Vymazat konfig. subor z adresara /etc/ld.so.conf.d/cuda-10.2.conf a potvrdit prikazom sudo ldconfig
1. Install [cuDNN 7 for CUDA 10.2](https://developer.nvidia.com/rdp/cudnn-download) (hlavickovy subor a kniznice sa musia prekopirovat do instalacneho priecinku s CUDA)
1. V CMake treba nastavit vsetky cesty ku CUDA 10.2 a cuDNN 7.
1. Set Nvidia host compiler to gcc-8.
1. Set CMake install prefix to /usr/local.
1. Configure
1. Generate
1. make all
1. sudo make install
