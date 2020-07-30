# Secure-File-Transfer-Protocol-Using-RSA-Encryption
This repository is about transferring the secure data from one computer to another with the help of socket programming using client-server architecture. The data will be secured by implementing RSA(cryptography) Algorithm. For simplicity only 64-bit security is used unlike real implementation which uses 128-bit to 256-bit security(used by banks,mililtary etc.).<br />
Client request for the file to server, with its name and a public key, generated by client itself. If the file is available to the server it will encrypt it with public key and send 'encrypted file' instead of original file to the client. Server in turn will decrypt the received 'encrypted file' with its own private key.<br />
## Key Features and install instructions:
1. You can have client at say system-1 and Server at say system-2.
2. You can create executable by compiling respective client and server programs i.e.: $ gcc client.c -o cli and then $ gcc server.c -o ser
3. Run 'server' excutable at system-2 with port address you want to assign for transmission. i.e.: ./ser 3000
4. When server is established, Run 'client' executable on system-1 with ip-address of server, filename of requested file and port number used by server. i.e. if we consider client and server are on same system then ip would be 127.0.0.1: ./cli 127.0.0.1  message.txt 3000
5. Bingo there will be a file with filename you requested in your 'client' folder.
