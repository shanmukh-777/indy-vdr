##build indy-vdr shared library
cd indy-vdr ##move inside vdr library
cargo build

##check whether library built
cd tager/debug  ##move inside debug
##check for linindy_vdr.so file

##export the path of .so file
export LD_LIBRARY_PATH=/home/shanmukh/Documents/go-aries/indy-vdr/target/debug/

##after that move inside wrapper/goland directory and check readme.md file
  ### first cp libindy_vdr.so file inside /usr/local/lib
  then you need to generate header file libindy_vdr.h following commands inside indy-vdr/libindy_vdr/include/Readme.md
  ## move that generated file to /usr/local/include inside

## after above steps you can simply run 
cd wrappers/golang
go run cmd/demo/demo.go
  
