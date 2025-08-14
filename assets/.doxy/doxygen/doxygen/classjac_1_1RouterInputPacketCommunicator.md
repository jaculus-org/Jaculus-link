

# Class jac::RouterInputPacketCommunicator



[**ClassList**](annotated.md) **>** [**jac**](namespacejac.md) **>** [**RouterInputPacketCommunicator**](classjac_1_1RouterInputPacketCommunicator.md)








Inherits the following classes: [jac::InputPacketCommunicator](classjac_1_1InputPacketCommunicator.md),  [jac::Consumer](classjac_1_1Consumer.md)










































































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**RouterInputPacketCommunicator**](#function-routerinputpacketcommunicator) () <br> |
| virtual size\_t | [**available**](#function-available) () override<br>_Get the number of packets available to read._  |
| virtual void | [**cancelRead**](#function-cancelread) () override<br>_Cancel any blocking read._  |
| virtual void | [**clear**](#function-clear) () override<br>_Clear the buffer._  |
| virtual std::optional&lt; std::pair&lt; int, std::vector&lt; uint8\_t &gt; &gt; &gt; | [**get**](#function-get) () override<br>_Get the next packet._  |
| virtual void | [**processPacket**](#function-processpacket) (int linkId, std::span&lt; const uint8\_t &gt; data) override<br> |


## Public Functions inherited from jac::InputPacketCommunicator

See [jac::InputPacketCommunicator](classjac_1_1InputPacketCommunicator.md)

| Type | Name |
| ---: | :--- |
|   | [**InputPacketCommunicator**](classjac_1_1InputPacketCommunicator.md#function-inputpacketcommunicator-12) () = default<br> |
|   | [**InputPacketCommunicator**](classjac_1_1InputPacketCommunicator.md#function-inputpacketcommunicator-22) (const [**InputPacketCommunicator**](classjac_1_1InputPacketCommunicator.md) &) = delete<br> |
| virtual size\_t | [**available**](classjac_1_1InputPacketCommunicator.md#function-available) () = 0<br>_Get the number of packets available to read._  |
| virtual void | [**cancelRead**](classjac_1_1InputPacketCommunicator.md#function-cancelread) () = 0<br>_Cancel any blocking read._  |
| virtual void | [**clear**](classjac_1_1InputPacketCommunicator.md#function-clear) () = 0<br>_Clear the buffer._  |
| virtual std::optional&lt; std::pair&lt; int, std::vector&lt; uint8\_t &gt; &gt; &gt; | [**get**](classjac_1_1InputPacketCommunicator.md#function-get) () = 0<br>_Get the next packet._  |
|  [**InputPacketCommunicator**](classjac_1_1InputPacketCommunicator.md) & | [**operator=**](classjac_1_1InputPacketCommunicator.md#function-operator) (const [**InputPacketCommunicator**](classjac_1_1InputPacketCommunicator.md) &) = delete<br> |
| virtual  | [**~InputPacketCommunicator**](classjac_1_1InputPacketCommunicator.md#function-inputpacketcommunicator) () = default<br> |


## Public Functions inherited from jac::Consumer

See [jac::Consumer](classjac_1_1Consumer.md)

| Type | Name |
| ---: | :--- |
|   | [**Consumer**](classjac_1_1Consumer.md#function-consumer-13) () = default<br> |
|   | [**Consumer**](classjac_1_1Consumer.md#function-consumer-23) (const [**Consumer**](classjac_1_1Consumer.md) &) = delete<br> |
|   | [**Consumer**](classjac_1_1Consumer.md#function-consumer-33) ([**Consumer**](classjac_1_1Consumer.md) &&) = delete<br> |
|  [**Consumer**](classjac_1_1Consumer.md) & | [**operator=**](classjac_1_1Consumer.md#function-operator) (const [**Consumer**](classjac_1_1Consumer.md) &) = delete<br> |
|  [**Consumer**](classjac_1_1Consumer.md) & | [**operator=**](classjac_1_1Consumer.md#function-operator_1) ([**Consumer**](classjac_1_1Consumer.md) &&) = delete<br> |
| virtual void | [**processPacket**](classjac_1_1Consumer.md#function-processpacket) (int linkId, std::span&lt; const uint8\_t &gt; data) = 0<br> |
| virtual  | [**~Consumer**](classjac_1_1Consumer.md#function-consumer) () = default<br> |
















































































## Public Functions Documentation




### function RouterInputPacketCommunicator 

```C++
inline jac::RouterInputPacketCommunicator::RouterInputPacketCommunicator () 
```




<hr>



### function available 

_Get the number of packets available to read._ 
```C++
inline virtual size_t jac::RouterInputPacketCommunicator::available () override
```





**Returns:**

The number 





        
Implements [*jac::InputPacketCommunicator::available*](classjac_1_1InputPacketCommunicator.md#function-available)


<hr>



### function cancelRead 

_Cancel any blocking read._ 
```C++
inline virtual void jac::RouterInputPacketCommunicator::cancelRead () override
```



Implements [*jac::InputPacketCommunicator::cancelRead*](classjac_1_1InputPacketCommunicator.md#function-cancelread)


<hr>



### function clear 

_Clear the buffer._ 
```C++
inline virtual void jac::RouterInputPacketCommunicator::clear () override
```



Implements [*jac::InputPacketCommunicator::clear*](classjac_1_1InputPacketCommunicator.md#function-clear)


<hr>



### function get 

_Get the next packet._ 
```C++
inline virtual std::optional< std::pair< int, std::vector< uint8_t > > > jac::RouterInputPacketCommunicator::get () override
```





**Note:**

This method blocks until a packet is available.




**Returns:**

The packet 





        
Implements [*jac::InputPacketCommunicator::get*](classjac_1_1InputPacketCommunicator.md#function-get)


<hr>



### function processPacket 

```C++
inline virtual void jac::RouterInputPacketCommunicator::processPacket (
    int linkId,
    std::span< const uint8_t > data
) override
```



Implements [*jac::Consumer::processPacket*](classjac_1_1Consumer.md#function-processpacket)


<hr>

------------------------------
The documentation for this class was generated from the following file `src/jac/link/routerCommunicator.h`

