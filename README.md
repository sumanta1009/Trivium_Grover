# Trivium_Grover
Initially, I started implementing my work with IBM Qiskit 0.46 version. Later in 2024 Qiskit came with 1.0+ versions. Some of the functionalities in my codes implemented in 0.46 version won't work with 1.0+ versions. So, I provided my codes which are implemented in Qiskit 1.0.2 version.

# To get better visualization of the histograms presented in 'Trivium_Grover_3qK_Qiskit0.46.ipynb', 'Trivium_Grover_3qK_Qiskit1.0.2.ipynb', 'Trivium_Grover_4qK_Qiskit0.46.ipynb' and 'Trivium_Grover_4qK_Qiskit1.0.2.ipynb' run the following code fragment:
%matplotlib inline #if imported already in the previous cells, uncomment the line

from qiskit.visualization import plot_histogram #if imported already in the previous cells, uncomment the line

import matplotlib.pyplot as plt #if imported already in the previous cells, uncomment the line

figure = plot_histogram(counts, title = "Actual key {0} is represented in Qiskit as {1} below\n Actual key is successfully recovered with probability {2:.2f}".format(b[::-1],b,c/1024))

#Label the axes

ax = figure.gca()  # Get the current axis

ax.set_xlabel('Qubit String', fontsize=12)  # Set x-axis label

ax.set_ylabel('Count', fontsize=12)  # Set y-axis label
