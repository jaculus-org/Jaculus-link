

# Class jac::InputPacketCommunicator



[**ClassList**](annotated.md) **>** [**jac**](namespacejac.md) **>** [**InputPacketCommunicator**](classjac_1_1InputPacketCommunicator.md)



_Communicator interface that can be used to receive packets._ 

* `#include <communicator.h>`





Inherited by the following classes: [jac::RouterInputPacketCommunicator](classjac_1_1RouterInputPacketCommunicator.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**InputPacketCommunicator**](#function-inputpacketcommunicator-12) () = default<br> |
|   | [**InputPacketCommunicator**](#function-inputpacketcommunicator-22) (const [**InputPacketCommunicator**](classjac_1_1InputPacketCommunicator.md) &) = delete<br> |
| virtual size\_t | [**available**](#function-available) () = 0<br>_Get the number of packets available to read._  |
| virtual void | [**cancelRead**](#function-cancelread) () = 0<br>_Cancel any blocking read._  |
| virtual void | [**clear**](#function-clear) () = 0<br>_Clear the buffer._  |
| virtual std::optional&lt; std::pair&lt; int, std::vector&lt; uint8\_t &gt; &gt; &gt; | [**get**](#function-get) () = 0<br>_Get the next packet._  |
|  [**InputPacketCommunicator**](classjac_1_1InputPacketCommunicator.md) & | [**operator=**](#function-operator) (const [**InputPacketCommunicator**](classjac_1_1InputPacketCommunicator.md) &) = delete<br> |
| virtual  | [**~InputPacketCommunicator**](#function-inputpacketcommunicator) () = default<br> |




























## Public Functions Documentation




### function InputPacketCommunicator [1/2]

```C++
jac::InputPacketCommunicator::InputPacketCommunicator () = default
```




<hr>



### function InputPacketCommunicator [2/2]

```C++
jac::InputPacketCommunicator::InputPacketCommunicator (
    const InputPacketCommunicator &
) = delete
```




<hr>



### function available 

_Get the number of packets available to read._ 
```C++
virtual size_t jac::InputPacketCommunicator::available () = 0
```





**Returns:**

The number 





        

<hr>



### function cancelRead 

_Cancel any blocking read._ 
```C++
virtual void jac::InputPacketCommunicator::cancelRead () = 0
```




<hr>



### function clear 

_Clear the buffer._ 
```C++
virtual void jac::InputPacketCommunicator::clear () = 0
```




<hr>



### function get 

_Get the next packet._ 
```C++
virtual std::optional< std::pair< int, std::vector< uint8_t > > > jac::InputPacketCommunicator::get () = 0
```





**Note:**

This method blocks until a packet is available.




**Returns:**

The packet 





        

<hr>



### function operator= 

```C++
InputPacketCommunicator & jac::InputPacketCommunicator::operator= (
    const InputPacketCommunicator &
) = delete
```




<hr>



### function ~InputPacketCommunicator 

```C++
virtual jac::InputPacketCommunicator::~InputPacketCommunicator () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `src/jac/link/communicator.h`

