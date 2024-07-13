# Chat Application

This is a chat application project developed for the Computer Networks course during the first semester of the 2022-2023 academic year at Ho Chi Minh City University of Technology. The application is built using Python and the Tkinter library for the user interface.

## Table of Contents
1. [System Architecture](#system-architecture)
2. [Center Server](#center-server)
3. [Peer](#peer)
4. [File Transfer](#file-transfer)
5. [Contributors](#contributors)

## System Architecture
The system uses a hybrid architecture consisting of one center server and multiple peers. The center server keeps track of the online status of peers, while peers communicate directly with each other for messaging and file transfer.

## Center Server
The center server monitors and updates the list of online peers. Peers need to ping the center server at regular intervals; otherwise, they will be disconnected.

### Starting the Center Server
To start the center server, run the following command:
```bash
python center-server.py
```

## Peer
Each peer acts as both a server and a client when communicating with other peers.

### Starting a Peer
To start a peer, run the following command:
```bash
python client.py
```
Users can log in with their username and password. If they do not have an account, they can sign up for a new one.

## File Transfer

### Sender
To send a file, type the following command in the chat box:
```bash
\file_transfer _PATH
```
Replace `_PATH` with the path to the file you want to send.

### Receiver
To receive a file, set the destination folder in the `GUI` class.

## Contributors
- **Đỗ Huy Hoàng**: Report writing, file transfer code
- **Võ Mạnh Quyền**: GUI coding, peer client code, peer server code
- **Trần Quang Thắng**: Center server code, peer server code
- **Mã Hoàng Khôi Nguyên**: Report writing
