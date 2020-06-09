Failure on Raspberry Pi 3 (Raspbian, based on Debian buster, 32-bit):

~~~
mkdir build
cd build
cmake ..
~~~

Error message:

~~~
-- The CXX compiler identification is GNU 8.3.0
-- Check for working CXX compiler: /usr/bin/c++
-- Check for working CXX compiler: /usr/bin/c++ -- works
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Detecting CXX compile features
-- Detecting CXX compile features - done
-- Could NOT find Mathematica_MathLink (missing: Mathematica_MathLink_LIBRARY Mathematica_MathLink_INCLUDE_DIR) 
-- Could NOT find Mathematica_WolframLibrary (missing: Mathematica_WolframLibrary_LIBRARY) (found version "5")
-- Found Mathematica_JLink: /opt/Wolfram/WolframEngine/12.0/SystemFiles/Links/JLink (found version "4.9.1") 
-- Could NOT find Mathematica_MUnit (missing: Mathematica_MUnit_PACKAGE_DIR) 
-- Found Mathematica: /opt/Wolfram/WolframEngine/12.0 (found suitable version "12.0.0", minimum required is "8.0") 
CMake Error at CMakeLists.txt:9 (Mathematica_ADD_LIBRARY):
  Unknown CMake command "Mathematica_ADD_LIBRARY".


-- Configuring incomplete, errors occurred!
See also "/home/pi/packages/test-FindMathematica/build/CMakeFiles/CMakeOutput.log".
~~~
