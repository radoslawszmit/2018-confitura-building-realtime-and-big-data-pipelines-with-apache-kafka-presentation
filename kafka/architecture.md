
# Architektura

+++
### Zero-copy
"Zero-copy" describes computer operations in which the CPU does not perform the task of copying data from one memory area to another. This is frequently used to save CPU cycles and memory bandwidth when transmitting a file over a network. Wikipedia



+++
### Data copying

@div[left-50 fragment]
![](img/traditional-data-copying.gif)
@divend

@div[right-50 fragment]
![](img/zero-copy-data-copying.gif)
@divend

<span class="footer">https://www.ibm.com/developerworks/library/j-zerocopy/index.html</span>



+++
### Context switching

@div[left-50 fragment]
![](img/traditional-context-switching.gif)
@divend

@div[right-50 fragment]
![](img/zero-copy-context-switching.gif)
@divend

<span class="footer">https://www.ibm.com/developerworks/library/j-zerocopy/index.html</span>