app1
====

app 
2  sudo dpkg cuda-repo-ubuntu1604-10-2-local-10.2.89-440.33.01_1.0-1_amd64.deb
   93  sudo dpkg -i cuda-repo-ubuntu1604-10-2-local-10.2.89-440.33.01_1.0-1_amd64.deb
   94  sudo apt-key add /var/cuda-repo-10-2-local-10.2.89-440.33.01/7fa2af80.pub
   95  sudo apt-get update
   96  sudo apt-get -y install cuda
   97  nvcc -v
   98  sudo gedit ~/.bashrc 
   99  sudo gedit /etc/profile
  100  sudo ldconfig
  101  reboot
  102  ls
  103  sudo chmod a+x reset_jetbrains_eval_mac_linux.sh 
  104  ls
  105  sudo ./reset_jetbrains_eval_mac_linux.sh 
  106  ./pycharm.sh 
  107  cat /proc/driver/nvidia/version 
  108  nvcc -V
  109  nvidia-smi 
  110  cd /usr/local/cuda/samples/1_Utilities/deviceQuery
  111  ls
  112  sudo make
  113  sudo ./deviceQuery 
  114  cd /usr/local/cuda-10.2/
  115  nautilus .
  116  sudo cp cudnn.h /usr/local/cuda-10.2/include/
  117  cd ..
  118  cd ..\
  119  sudo cp cuda/lib64/libcudnn* /usr/local/cuda-10.2/lib64/
  120  sudo chmod a+r /usr/local/cuda-10.2/include/cudnn.h 
  121  sudo chmod a+r /usr/local/cuda-10.2/lib64/libcudnn*
  122  sudo chmod -R 777 /usr/local/cuda-10.2/lib64/libcudnn*
  123  sudo chmod -R 777 /usr/local/cuda-10.2/include/cudnn.h 
  124  cat /usr/local/cuda-10.2/include/cudnn.h | grep CUDNN_MAJOR -A 2
  125  cd
  126  ls
  127  cd software/
  128  ls
  129  cd clion-2016.2.2/
  130  ls
  131  cd bin/
  132  ls
  133  sudo ./clion.sh 
  134  cd ../
  135  cd 
  136  ls
  137  cd software/clion-2020.3.2/
  138  ls
  139  cd bin/
  140  ls
  141  sudo ./clion.sh 
  142  sudo ./clion.sh 
  143  ps -ef
  144  ps -ef | grep clion
  145  sudo ./clion.sh 
  146  pwd
  147  pwd
  148  cd software/clion-2020.3.2/bin/
  149  sudo ./clion.sh 
  150  cd ../../
  151  ls
  152  cd pycharm-2020.3/bin/
  153  sudo ./pycharm.sh 
  154  python3
  155  pip install tensorflow==1.12.0
  156  pip install keras==2.2.4
  157  sudo add-apt-repository ppa:jonathonf/python-3.6
  158  sudo apt-get update
  159  python
  160  sudo apt-get install python3.6
  161  sudo apt-get update
  162  pip install tensorflow-gpu keras
  163  pip install tensorflow==2.1.0 keras==2.3.1
  164  pip install tensorflow-gpu==2.1.0 keras==2.3.1
  165  nvidia-smi
  166  nvidia-smi -l 1
  167  wget http://www.python.org/ftp/python/3.6.4/Python-3.6.4.tgz
  168  ls
  169  mv Python-3.6.4.tgz software/
  170  cd software/
  171  ls
  172  tar -xvzf Python-3.6.4.tgz
  173  cd Python-3.6.4/
  174  ./configure --with-ssl
  175  sudo make
  176  sudo make install
  177  sudo apt-get install zlib* 
  178  sudo make install
  179  which python3
  180  sudo  ln -s /usr/local/bin/python3 python
  181  python3
  182  python
  183  sudo dpkg -i cuda-repo-ubuntu1604-10-0-local-10.0.130-410.48_1.0-1_amd64.deb 
  184  sudo dpkg -i cuda-repo-ubuntu1604-10-0-local-10.0.130-410.48_1.0-1_amd64.deb
  185  cd /usr/local/
  186  ls
  187  cd 
  188  nvidia-smi 
  189  nvidia-smi -l 1
  190  sudo apt-get remove cuda
  191  sudo apt-get remove cuda*
  192  cd /usr/local
  193  dir
  194  sudo rm -r cuda-10.2/
  195  ls
  196  sudo dpkg -i cuda-repo-ubuntu1604-10-0-local-10.0.130-410.48_1.0-1_amd64.deb
  197  nvidia-smi 
  198  reboot
  199  systemctl reboot -i
  200  nvidia-smi
  201  sudo dpkg -i cuda-repo-ubuntu1604-10-0-local-10.0.130-410.48_1.0-1_amd64.deb
  202  sudo apt-key add /var/cuda-repo-10-0-local/7fa2af80.pub
  203  sudo apt-get --purge remove "*cublas*" "cuda*"
  204  sudo dpkg -i cuda-repo-ubuntu1604-10-0-local-10.0.130-410.48_1.0-1_amd64.deb
  205  sudo apt-key add /var/cuda-repo-10-0-local/7fa2af80.pub
  206  sudo apt autoremove 
  207  dpkg -l | grep ^rc | awk '{print $2}'|sudo xargs dpkg -P
  208  dpkg -l | grep nvidia | awk '{print $2}'|sudo xargs dpkg -P
  209  sudo apt-get remove cuda
  210  dpkg -l | grep cuda | awk '{print $2}'|sudo xargs dpkg -P
  211  sudo service lightdm stop 
  212  lshw -numeric -C display
  213  cd Downloads/
  214  chmod a+x NVIDIA-Linux-x86_64-460.39.run 
  215  ls
  216  sudo ./NVIDIA-Linux-x86_64-460.39.run –no-x-check –no-nouveau-check –no-opengl-files
  217  sudo ./NVIDIA-Linux-x86_64-460.39.run  –no-nouveau-check –no-opengl-files
  218  ubuntu-drivers devices
  219  sudo ubuntu-drivers autoinstall
  220  sudo ./NVIDIA-Linux-x86_64-460.39.run -no-x-check -no-nouveau-check -no-opengl-files
  221  reboot
  222  nvidia-smi
  223  cd Downloads/
  224  sudo ./NVIDIA-Linux-x86_64-460.39.run --uninstall
  225  sudo ./NVIDIA-Linux-x86_64-460.39.run -no-opengl-files
  226  sudo service lightdm stop
  227  cd /etc/modprobe.d/
  228  ls
  229  sudo gedit /etc/modprobe.d/blacklist.conf 
  230  sudo update-initramfs -u
  231  lsmod | grep nouveau
  232  reboot
  233  lsmod | grep nouveau
  234  ls
  235  cd Downloads/
  236  ls
  237  sudo ./NVIDIA-Linux-x86_64-460.39.run -no-x-check -no-nouveau-check -no-opengl-files
  238  sudo service lightdm start 
  239  nvidia-smi 
  240  nvidia-settings 
  241  sudo dpkg -i cuda-repo-ubuntu1604-10-0-local-10.0.130-410.48_1.0-1_amd64.deb
  242  sudo apt-key add /var/cuda-repo-10-0-local-10.0.130-410.48/7fa2af80.pub
  243  sudo apt-get update
  244  sudo apt-get install cuda
  245  sudo chmod -R 777 cudnn.h 
  246  sudo gedit ~/.bashrc 
  247  sudo gedit /etc/profile
  248  cd /usr/local/cuda-10.0/samples/1_Utilities/deviceQuery
  249  sudo make
  250  ./deviceQuery 
  251  reboot
  252  sudo cp libcudnn* /usr/local/cuda-10.0/lib64/ -rf
  253  cd ../include/
  254  ls
  255  sudo cp cudnn.h /usr/local/cuda-10.0/include
  256  chmod a+r 777 libcudnn*
  257  sudo chmod a+r 777 libcudnn*
  258  sudo chmod -R 777 libcudnn*
  259  top -h 1
  260  top -d 1
  261  pip install tensorflow-gpu==2.0.0
  262  export CUDA_VISIBLE_DEVICES=0
  263  python testGpu.py 
  264  pip install keras==2.3.1
  265  nvidia-smi 
  266  nvidia-smi -l 1
  267  pip list tensorflow
  268  pip list keras
  269  pip install --upgrade --force-reinstall tensorflow-gpu
  270  pip install --upgrade --force-reinstall tensorflow-gpu==2.1.0
  271  nvcc --version
  272  nvidia-smi 
  273  nvidia-smi -l 1
  274  git clone https://github.com/Hoke/WebrtcAudioMixer.git
  275  cd 
  276  cd software/clion-2020.3.2/bin/
  277  sudo ./clion.sh 
  278  java 
  279  sudo ./clion.sh 
  280  sudo ./clion.sh --disable-gpu
  281  sudo ./clion.sh
  282  git clone https://github.com/zhangwei147258/safety_helmet_detect_retinanet_keras.git
  283  sudo apt install git
  284  git clone https://github.com/zhang527/webrtcTransport.git
  285  git clone --depth 1 https://gitee.com/xia-chu/ZLMediaKit
  286  cd ZLMediaKit/
  287  git submodule update --init
  288  sudo apt-get install build-essential
  289  sudo apt-get install cmake
  290  ls
  291  cd media_code/
  292  ls
  293  rm WebrtcAudioMixer/ -rf
  294  sudo rm WebrtcAudioMixer/ -rf
  295  git clone https://github.com/Hoke/wms.git
  296  ls
  297  cd
  298  ls
  299  cd ffmpeg_source/
  300  ls
  301  git -C fdk-aac pull 2> /dev/null || git clone --depth 1 https://github.com/mstorsjo/fdk-aac && cd fdk-aac && autoreconf -fiv && ./configure --prefix="$HOME/ffmpeg_build" --disable-shared && make && make install
  302  git -C opus pull 2> /dev/null || git clone --depth 1 https://github.com/xiph/opus.git && cd opus && ./autogen.sh && ./configure --prefix="$HOME/ffmpeg_build" --disable-shared && make && make install
  303  ls
  304  rm opus/ -rf
  305  cd ..
  306  ls
  307  git -C opus pull 2> /dev/null || git clone --depth 1 https://github.com/xiph/opus.git && cd opus && ./autogen.sh && ./configure --prefix="$HOME/ffmpeg_build" --disable-shared && make && make install
  308  ls
  309  ./autogen.sh 
  310  cd ..
  311  sudo apt-get install autoconf automake libtool
  312  cd opus/
  313  git -C opus pull 2> /dev/null || git clone --depth 1 https://github.com/xiph/opus.git && cd opus && ./autogen.sh && ./configure --prefix="$HOME/ffmpeg_build" --disable-shared && make && make install
  314  cd ..
  315  ls
  316  cd ..
  317  ls
  318  mv ffmpeg-4.3.1 ffmpeg
  319  ls
  320  cd ffmpeg/
  321  ls
  322  cd ..
  323  cd ffmpeg && PATH="$HOME/bin:$PATH" PKG_CONFIG_PATH="$HOME/ffmpeg_build/lib/pkgconfig" ./configure --prefix="$HOME/ffmpeg_build" --pkg-config-flags="--static" --extra-cflags="-I$HOME/ffmpeg_build/include" --extra-ldflags="-L$HOME/ffmpeg_build/lib" --extra-libs="-lpthread -lm" --bindir="$HOME/bin" --disable-asm --disable-x86asm --disable-inline-asm --enable-decoder=aac --enable-decoder=aac_fixed --enable-decoder=aac_latm --enable-libfdk-aac --enable-decoder=libopus --enable-encoder=aac --enable-encoder=opus --enable-encoder=libopus --enable-libopus --enable-lzma --enable-libsrt --enable-libvpx --enable-encoder=libvpx_vp8 --enable-encoder=libvpx_vp9 --enable-decoder=vp8 --enable-decoder=vp9 --enable-parser=vp8 --enable-parser=vp9 --disable-dct --disable-dwt --disable-vaapi --disable-vdpau && PATH="$HOME/bin:$PATH" make && make install && hash -r
  324  ls
  325  cd ..
  326  ls
  327  cd fdk-aac && autoreconf -fiv && ./configure --prefix="$HOME/ffmpeg_build" --disable-shared && make && make install
  328  cd ..
  329  cd ffmpeg && PATH="$HOME/bin:$PATH" PKG_CONFIG_PATH="$HOME/ffmpeg_build/lib/pkgconfig" ./configure --prefix="$HOME/ffmpeg_build" --pkg-config-flags="--static" --extra-cflags="-I$HOME/ffmpeg_build/include" --extra-ldflags="-L$HOME/ffmpeg_build/lib" --extra-libs="-lpthread -lm" --bindir="$HOME/bin" --disable-asm --disable-x86asm --disable-inline-asm --enable-decoder=aac --enable-decoder=aac_fixed --enable-decoder=aac_latm --enable-libfdk-aac --enable-decoder=libopus --enable-encoder=aac --enable-encoder=opus --enable-encoder=libopus --enable-libopus --enable-lzma --enable-libsrt --enable-libvpx --enable-encoder=libvpx_vp8 --enable-encoder=libvpx_vp9 --enable-decoder=vp8 --enable-decoder=vp9 --enable-parser=vp8 --enable-parser=vp9 --disable-dct --disable-dwt --disable-vaapi --disable-vdpau && PATH="$HOME/bin:$PATH" make && make install && hash -r
  330  cd ..
  331  git clone https://github.com/Haivision/srt.git
  332  sudo apt-get install tclsh pkg-config cmake libssl-dev build-essential
  333  cd srt/
  334  ./configure
  335  make
  336  make install
  337  sudo make install
  338  cd ..
  339  cd ffmpeg && PATH="$HOME/bin:$PATH" PKG_CONFIG_PATH="$HOME/ffmpeg_build/lib/pkgconfig" ./configure --prefix="$HOME/ffmpeg_build" --pkg-config-flags="--static" --extra-cflags="-I$HOME/ffmpeg_build/include" --extra-ldflags="-L$HOME/ffmpeg_build/lib" --extra-libs="-lpthread -lm" --bindir="$HOME/bin" --disable-asm --disable-x86asm --disable-inline-asm --enable-decoder=aac --enable-decoder=aac_fixed --enable-decoder=aac_latm --enable-libfdk-aac --enable-decoder=libopus --enable-encoder=aac --enable-encoder=opus --enable-encoder=libopus --enable-libopus --enable-lzma --enable-libsrt --enable-libvpx --enable-encoder=libvpx_vp8 --enable-encoder=libvpx_vp9 --enable-decoder=vp8 --enable-decoder=vp9 --enable-parser=vp8 --enable-parser=vp9 --disable-dct --disable-dwt --disable-vaapi --disable-vdpau && PATH="$HOME/bin:$PATH" make && make install && hash -r
  340  sudo apt-get install liblzma-dev 
  341  cd ffmpeg && PATH="$HOME/bin:$PATH" PKG_CONFIG_PATH="$HOME/ffmpeg_build/lib/pkgconfig" ./configure --prefix="$HOME/ffmpeg_build" --pkg-config-flags="--static" --extra-cflags="-I$HOME/ffmpeg_build/include" --extra-ldflags="-L$HOME/ffmpeg_build/lib" --extra-libs="-lpthread -lm" --bindir="$HOME/bin" --disable-asm --disable-x86asm --disable-inline-asm --enable-decoder=aac --enable-decoder=aac_fixed --enable-decoder=aac_latm --enable-libfdk-aac --enable-decoder=libopus --enable-encoder=aac --enable-encoder=opus --enable-encoder=libopus --enable-libopus --enable-lzma --enable-libsrt --enable-libvpx --enable-encoder=libvpx_vp8 --enable-encoder=libvpx_vp9 --enable-decoder=vp8 --enable-decoder=vp9 --enable-parser=vp8 --enable-parser=vp9 --disable-dct --disable-dwt --disable-vaapi --disable-vdpau && PATH="$HOME/bin:$PATH" make && make install && hash -r
  342  cd ..
  343  cd ffmpeg && PATH="$HOME/bin:$PATH" PKG_CONFIG_PATH="$HOME/ffmpeg_build/lib/pkgconfig" ./configure --prefix="$HOME/ffmpeg_build" --pkg-config-flags="--static" --extra-cflags="-I$HOME/ffmpeg_build/include" --extra-ldflags="-L$HOME/ffmpeg_build/lib" --extra-libs="-lpthread -lm" --bindir="$HOME/bin" --disable-asm --disable-x86asm --disable-inline-asm --enable-decoder=aac --enable-decoder=aac_fixed --enable-decoder=aac_latm --enable-libfdk-aac --enable-decoder=libopus --enable-encoder=aac --enable-encoder=opus --enable-encoder=libopus --enable-libopus --enable-lzma --enable-libsrt --enable-libvpx --enable-encoder=libvpx_vp8 --enable-encoder=libvpx_vp9 --enable-decoder=vp8 --enable-decoder=vp9 --enable-parser=vp8 --enable-parser=vp9 --disable-dct --disable-dwt --disable-vaapi --disable-vdpau && PATH="$HOME/bin:$PATH" make && make install && hash -r
  344  cd ..
  345  cd srt/
  346  ls
  347  ./configure 
  348  make
  349  sudo make install
  350  pkg-config --list-all | grep srt
  351  cd ..
  352  cd ffmpeg && PATH="$HOME/bin:$PATH" PKG_CONFIG_PATH="$HOME/ffmpeg_build/lib/pkgconfig" ./configure --prefix="$HOME/ffmpeg_build" --pkg-config-flags="--static" --extra-cflags="-I$HOME/ffmpeg_build/include" --extra-ldflags="-L$HOME/ffmpeg_build/lib" --extra-libs="-lpthread -lm" --bindir="$HOME/bin" --disable-asm --disable-x86asm --disable-inline-asm --enable-decoder=aac --enable-decoder=aac_fixed --enable-decoder=aac_latm --enable-libfdk-aac --enable-decoder=libopus --enable-encoder=aac --enable-encoder=opus --enable-encoder=libopus --enable-libopus --enable-lzma --enable-libsrt --enable-libvpx --enable-encoder=libvpx_vp8 --enable-encoder=libvpx_vp9 --enable-decoder=vp8 --enable-decoder=vp9 --enable-parser=vp8 --enable-parser=vp9 --disable-dct --disable-dwt --disable-vaapi --disable-vdpau && PATH="$HOME/bin:$PATH" make && make install && hash -r
  353  cd ..
  354  cd ffmpeg && PATH="$HOME/bin:$PATH" PKG_CONFIG_PATH="$HOME/ffmpeg_build/lib/pkgconfig" ./configure --prefix="$HOME/ffmpeg_build" --pkg-config-flags="--static" --extra-cflags="-I$HOME/ffmpeg_build/include" --extra-ldflags="-L$HOME/ffmpeg_build/lib" --extra-libs="-lpthread -lm" --bindir="$HOME/bin" --disable-asm --disable-x86asm --disable-inline-asm --enable-decoder=aac --enable-decoder=aac_fixed --enable-decoder=aac_latm --enable-libfdk-aac --enable-decoder=libopus --enable-encoder=aac --enable-encoder=opus --enable-encoder=libopus --enable-libopus --enable-lzma  --enable-libvpx --enable-encoder=libvpx_vp8 --enable-encoder=libvpx_vp9 --enable-decoder=vp8 --enable-decoder=vp9 --enable-parser=vp8 --enable-parser=vp9 --disable-dct --disable-dwt --disable-vaapi --disable-vdpau && PATH="$HOME/bin:$PATH" make && make install && hash -r
  355  history
