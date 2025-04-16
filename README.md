# Second research internship at LFDQ (quantum devices physics laboratory) UNICAMP

In the first part of this internship I did a study on superconducting qubits that can be seen on my [final report](https://github.com/Danielgb23/ic-superconductor-qubit/blob/master/final_report_Daniel.pdf)
using as bibliography Gross [1] for the first part which is a study on the superconducting effect. Then, a study of circuit Quantum Electrodynamics (QED) using Girvin [2] 
where I went through the josephson junction, the quantum harmonic oscillator, the inharmony that using a Josephson junction in place of of an inductor causes creating 
an "artificial atom" qubit and the Jaynes-Cumming approximation of the Hamiltonian of the qubit coupled to a microwave cavity.

The second part I did several simulations. [The first notebook](https://github.com/Danielgb23/ic-superconductor-qubit/blob/master/2-qubit-gates.ipynb) simulates a
using Qutip a cavity plus two qubits system that is controlled to do a series of one gate and two gates operations. With this we obtain the equivalent of applying a 
CNOT gate plus some one qubit gate operations described with better details on the
notebook. References quoted in this notebook are Krantz’s [3] and Wolfowicz’s [4]. 
(In [this notebook](https://github.com/Danielgb23/ic-superconductor-qubit/blob/master/cavity-qubit%20gates.ipynb) 
I basically do the same but play with a cavity using Jaynes-Cumming).

![image](https://github.com/user-attachments/assets/2c985e0e-5e7b-4baf-bdc0-bd0d48b91af1)

![image](https://github.com/user-attachments/assets/ce0bec17-44a0-4177-ba19-7bd2bc89d301)

In [the second notebook](https://github.com/Danielgb23/ic-superconductor-qubit/blob/master/finding%20g%20the%20interaction%20factor.ipynb)  we simulate two qubits and vary the frequency of one of them
to measure the amount of interaction it has with one another. In this case with a iSWAP gate like used
before. Then we vary the time they interact and conduct a measurement from whose
period of variation of the state transfer we can find the g interaction factor. This is
supposed to emulate a common process of calibration of this factor in a real quantum
computer. 

![image](https://github.com/user-attachments/assets/53c86be5-ed8f-4238-a5cb-a2d5f3fc3b67)


In [the third notebook](https://github.com/Danielgb23/ic-superconductor-qubit/blob/master/Measurement.ipynb)
of the simulations we emulate the process of conducing a measurement through a cavity.
For that we drive the cavity with a cosine wave and read the reflected/transmitted back
wave with the expected value for the a operator of the cavity. Different states of the qubit will
result in waves with different frequency as explained further in the notebook.

![image](https://github.com/user-attachments/assets/0b738e21-e3f7-4a0a-833e-19469f360f65)


Finally, using the tool from IBM, qiskit metal. I studied and modified two notebooks available
from IBM tutorials:

- [Design a 4 qubit full chip](https://github.com/Qiskit/qiskit-metal/blob/main/tutorials/2%20From%20components%20to%20chip/C.%20My%20first%20full%20quantum%20chip%20design/2.21%20Design%20a%204%20qubit%20full%20chip.ipynb)
- [Two Crossmons Tunable Coupler](https://qiskit.org/documentation/metal/circuit-examples/D.Qubit-couplers/31-TwoCrossmonsTunableCoupler.html)

Creating with these two tutorials a notebook for two transmon qubits coupled by a
[cavity](https://github.com/Danielgb23/ic-superconductor-qubit/blob/master/Design%20a%202%20qubit%20full%20chip.ipynb)
and another notebook for the transmons coupled by a [coupler qubit](https://github.com/Danielgb23/ic-superconductor-qubit/blob/master/TwoTransmonsTunableCoupler.ipynb).

![image](https://github.com/user-attachments/assets/17f8cfcc-f536-41de-a2d0-93fb5afd2930)


[1] R. Gross, A. Marx, F. Deppe, Applied Superconductivity: Josephson Effect
and Superconducting Electronics, Walter De Gruyter Incorporated, 2016.

[2] S. M. Girvin, R. J. Schoelkopf in, 2015.

[3] P. Krantz, M. Kjaergaard, F. Yan, T. P. Orlando, S. Gustavsson, W. D.
Oliver, Applied Physics Reviews 2019, 6, 021318.

[4] G. Wolfowicz, J. J. Morton in eMagRes, Vol. 5, 4, John Wiley & Sons, Ltd,
Chichester, UK, 2016, pp. 1515–1528.
