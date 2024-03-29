# sample_netconf_connection
How to connect to device through netconf and get data. 

The Network Configuration Protocol (NETCONF) is a network management protocol developed and standardized by the IETF. It was developed in the NETCONF working group[1] and published in December 2006 as RFC 4741[2] and later revised in June 2011 and published as RFC 6241.[3] The NETCONF protocol specification is an Internet Standards Track document.

NETCONF provides mechanisms to install, manipulate, and delete the configuration of network devices. Its operations are realized on top of a simple Remote Procedure Call (RPC) layer. The NETCONF protocol uses an Extensible Markup Language (XML) based data encoding for the configuration data as well as the protocol messages. The protocol messages are exchanged on top of a secure transport protocol.

The NETCONF protocol can be conceptually partitioned into four layers:

The Content layer consists of configuration data and notification data.
The Operations layer defines a set of base protocol operations to retrieve and edit the configuration data.
The Messages layer provides a mechanism for encoding remote procedure calls (RPCs) and notifications.
The Secure Transport layer provides a secure and reliable transport of messages between a client and a server.

NETCONF PROTOCOL LAYERS

![image](https://user-images.githubusercontent.com/94804863/160762208-6150387f-2d54-4f82-805e-416449017a5e.png)

NETCONF uses SSH port number 830 as the default port. The port number is a configurable option. NETCONF also supports capability discovery and model downloads. 

The following command is used to say hello to the device, the port 830 is used to connect through Netconf. 



# ssh netcfg_user@172.29.6.186 -p 830 -s  netconf 

netcfg_user is netconf user. 
