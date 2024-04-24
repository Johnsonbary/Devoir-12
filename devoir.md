    ------------o INSTALLER MYSQL o-------------------

      $ tar -zxvf mysql-8.3.0.tar.gz
      $ cd mysql-8.3.0
      $ cat README.md
      $ mkdir build
      $ cd build
      $ cmake ..
      error1: command not found
      $ sudo apt install cmake
      $ cmake ..
      error: boost not found
      $ cd ..
      $ tar -jxvf boost_1_77_0.tar.bz2
      $ cd boost_1_77_0
      $ ./boostrap.sh
      $ ./b2
      $ ./b2 install
      $ cd ../mysql-8.3.0/build
      $ cmake ..
      error1: ncurses not found
      $ cd ../..
      $ tar -zxvf ncurses-6.4.tar.gz
      $ cd ncurses-6.4
      $ cat README
      $ ./configure
      $ make
      $ sudo make install
      $ cd ../mysql-8.3.0/build
      $ cmake ..
      $ make
      $ sudo make install



    ------------o INSTALLER APACHE o------------------
      $ tar -zxvf httpd-2.4.59.tar.gz
      $ cd httpd-2.4.59
      $ cat README
      $ ./configure
      error1: APR not found 
      $ sudo apt install libapr1-dev
      $ ./configure
      error1: APR-util not found
      $ sudo apt install libaprutil1-dev
      $ ./configure
      $ make 
      $ sudo make install



    --------------o INSTALLER PHP o-------------------
      $ tar -zxvf php-8.3.6.tar.gz
      $ cd php-8.3.6
      $ cat README.md
      $ ./configure
      error1: xml not found
      $ sudo apt install libxml2-dev
      $ ./configure
      error1: sqlite not found
      $ sudo apt install sqlite3-dev
      $ ./configure
      error1: pcre not found
      $ sudo apt install libpcre3-dev 
      $ ./configure
      error1: openssl not found
      $ sudo apt install libssl-dev
      $ ./configure
      $ sudo apt install zlib1g-dev 
      $ ./configure
      $ make 
      $ sudo make install	
