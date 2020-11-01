## What is heartbleed bug?

It is a vulnerability in OpenSSL software library that allows anyone on the Internet to read the memory of the systems. The attacker in worst case can get hold of security passwords, certificate keys which were available in-memory. 

## What was the vulnerability?

```
struct {
      HeartbeatMessageType type;
      uint16 payload_length;
      opaque payload[HeartbeatMessage.payload_length];
      opaque padding[padding_length];
   } HeartbeatMessage;
```


## How can an attacker exploit it?




## References
1. [RFC-6520: Transport Layer Security (TLS) and Datagram Transport Layer Security (DTLS) Heartbeat Extension](https://tools.ietf.org/html/rfc6520)
2. https://www.youtube.com/watch?v=1dOCHwf8zVQ
2. [Bug fix commit](https://github.com/openssl/openssl/commit/731f431497f463f3a2a97236fe0187b11c44aead)

