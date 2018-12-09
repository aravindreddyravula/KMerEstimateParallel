Hardware Specifications:

OS - Windows 10

RAM - 8GB

Software Specifications:

C++11

Cygwin

Sublime Text Editor


Note: Install zlib package which is necessary for compression(In our case hashing)




Compile and Run Serial Implementation
------------------------------


Compile:


		g++ kmerCountEstimate_serial.cpp -lpthread -lz -std=c++11
		
		
Run:


		./a.exe -f <seq.fa> -k  <kmerLen> -s <minHeap_Size> -c <coverage> -o <out.txt>
  
 Compile and Run Parallel Implementation
------------------------------ 


Compile:


		g++ kmerCountEstimate_parallel.cpp FastxParser.cpp -lpthread -lz -std=c++11
		
		
Run:


		./a.exe -f <seq.fa> -k  <kmerLen> -s <minHeap_Size> -c <coverage> -o <out.txt> -np<NoOfProducers> -nt <NoOfConsumers> 
  
