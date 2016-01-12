NIO(Non blocking IO)

* It was introduced in Java7. It is an alternative IO API for java(introduced in java 1.4)
* In IO API we work with byte streams and character streams, whereas in NIO package we deal with buffers and channels by which data is always read from a channel into a buffer or written from a buffer to a channel.
* It defines buffers, which are considered to be the containers for data.
* There are several other packages that comes under nio package.
* The basic core components of NIO package includes buffers, charset, channels and selectors.

Channels and buffers : These comes under java.nio package where data is always read from a channel into a buffer or written to a channel from a buffer.

Java Non blocking IO : It enables us to perform non blocking IO operations, example a thread can ask a channel to read data into a buffer and at the same time thread can do somthing else; once the operation is finished the thread can ressume its operation.

Selectors : These are objects which monitors multiple channels for events.

The list of channel implementations are 

* FileChannel
* DatagramChannel
* SocketChannel
* ServerSocketChannel

These channels cover UDP ,TCP and file IO    

The implementaion classed for buffers include:

* ByteBuffer
* CharBuffer
* DoubleBuffer
* FloatBuffer
* IntBuffer
* LongBuffer
* ShortBuffer

A few Differences between IO and NIO are:
* We can both read and write to a channel, whereas Streams are unidirectional.
* Channels can be read or write asynchronously.
* Channels always read to or write from a buffer.

Channel Implementaitons :

* The FileChannel reads data from and to files.
* The DatagramChannel can read and write data over the network via UDP.
* The SocketChannel can read and write data over the network via TCP.
* The ServerSocketChannel allows you to listen for incoming TCP connections, like a web server does. For each incoming connection a SocketChannel is created.