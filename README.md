# Quantum
quantum computer using C++

Quantum is a library of functions and classes for simulating the action of a quantum
computer using C++. It contains two classes - QubitSystem and QuantumGate - that
simulate the two primary structures used in quantum computing, quantum bits 
(qubits) and gates that operate on systems of one or more qubits. 

Encapsulation is used to enforce the limitations that make programming for a 
quantum computer fundamentally different than for a classical computer. The 
operations that can be performed on an object of the class QubitSystem, which 
represents a system of one or more possibly entangled qubits, are essentially 
limited to applying the action of a unitary quantum gate on the system and 
"observing" the system, which collapses it to a pure state. This allows the user
to design, implement, and test algorithms in a natural way under the constraints
inherent to quantum computing. 

The QAS library has an extremely compact and intuitive interface, making it easy
to learn and use for anyone familiar with C++. It fits easily within a larger 
C++ program, so that mixing classical and quantum programming is effortless. For
examples of use, see the unit tests in the test/ directory. 


Dependencies: 
-GNU Scientific Library (GSL)
-Basic Linear Algebra Subprograms (BLAS)
-CMake 

The following dependencies are needed only in order to be able to run the unit 
tests:
-Google Test
-Pthreads 

Contact: adysenlab@gmail.com

[Talk to our dev team](https://join.slack.com/t/adysenlab/shared_invite/enQtNDIwMjkwNDU4NjQ3LTM0ZmQwYmNmNDBlNWJjZTVjOGU0Y2RhYTM2ZjBhNmYzZDEwMjFhMmY5ZDIzYWQ3NjEyYzNkZGI3YWViMzY1NjY)
# Installation instructions
----------------------------

Scripts are provided for installing QAS using CMake. To install: 
1. Edit any of the CMakeLists.txt files (located in the main directory, lib/, 
   and test/) as necessary. 
2. Navigate to the build/ directory. 
3. Configure and auto-generate a Makefile by typing:
   $ cmake ..

4. Generate the library and test executable by typing:
   $ make

5. Optionally, run the test suite by navigating to the test/ directory and
   typing:
   $ ./run_tests