# LocalSOCKS5DPIBYPASS

Local SOCKS5 DPI BYPASS.
[PC](https://github.com/Therapist191124/LocalSOCKS5DPIBYPASS?tab=readme-ov-file#pc)
[Android](https://github.com/Therapist191124/LocalSOCKS5DPIBYPASS?tab=readme-ov-file#android)

## Is it Working :
![2025-02-20_10-17-27](https://github.com/user-attachments/assets/517212a0-4bc7-4a2a-9692-deeaeaf835b0)

## Before You start:
- As a local proxy, it doesn't require complex setup or external infrastructure.
  
- End-to-End Encryption: It does not inherently provide encryption. Users should combine it with secure protocols like HTTPS or VPNs for comprehensive protection.
  
- Effective Against DPI Filters: Successfully bypasses many forms of network-level filtering and throttling.
  
- Customizable Options: Offers fine-grained control over how traffic is obfuscated, allowing users to adapt to different blocking mechanisms.
  
- Obfuscating Traffic: It modifies the structure of network packets to confuse DPI systems, making it harder for them to identify and block specific protocols or content.
  
- Maintaining Privacy: By altering packet headers and payloads, it prevents ISPs or network administrators from inspecting user activity in detail.

## PC
### Requirements

[ByeDPI](https://github.com/hufrea/byedpi) to create the server. 

[Nekoray](https://github.com/MatsuriDayo/nekoray).

[v2rayN (Alternative to Nekoray)](https://github.com/2dust/v2rayN).

Download them and unzip.

### Steps :
#### 1. ByeDPI.
1. Go to ByeDPI folder.
2. Run service_install.bat (Run as administrator) and it will be istalled automatically.
3. Find byedpi.bat file and edit it (Open as notepad).
   ![2025-02-20_09-32-25](https://github.com/user-attachments/assets/ef0df219-8044-43e1-913a-0d96de7c1c2b)
4. Replace the existing parameter with this one :
   ![2025-02-20_09-33-33](https://github.com/user-attachments/assets/9bf6ffff-92e9-471d-a316-0ed820752aef)

```bash
ciadpi.exe --fake -2 --tls-sni Ea.com --tlsrec 6+s --tlsrec 27+s
```
5. Save it.
 ![2025-02-20_09-35-16](https://github.com/user-attachments/assets/947d8729-157c-4688-9876-6e9aa6090534)
6. Open byedpi.bat.
   ![2025-02-20_09-37-17](https://github.com/user-attachments/assets/3e323731-2973-4b8a-ad4a-e00c7b61ee4d)
   ![2025-02-20_09-37-51](https://github.com/user-attachments/assets/9d80dd4e-00e8-4a80-9b65-fe6b9e60c46e)


#### 2. Nekoray.
1. Go to Nekoray folder.
2. Open Nekobox.exe file.
   ![2025-02-20_09-38-42](https://github.com/user-attachments/assets/a2b05f71-20cc-42bf-b429-ac64c2168c90)
3. Add new Profile :
   ![2025-02-20_09-43-41](https://github.com/user-attachments/assets/57a561fa-8e5f-418e-927c-1ebc18d0ade5)
   ![2025-02-20_09-44-35](https://github.com/user-attachments/assets/c3bfc009-c97b-46e2-9d77-a9f29321660f)
```bash
socks5://127.0.0.1:1080
```
4. Enable system proxy.
   ![2025-02-20_09-45-15](https://github.com/user-attachments/assets/de0e4af1-099c-407d-a73d-83c0dcf3fef9)
5. Run it.
   ![2025-02-20_09-46-22](https://github.com/user-attachments/assets/031f1fc4-0653-422d-9b03-15a7de34f339)
### Confirmation :
1. Check the opened CMD terminal (Byedpi.bat), and make sure it is not giving you any error.
   ![2025-02-20_09-47-46](https://github.com/user-attachments/assets/6409b552-cbf7-4f1c-a11f-12ebe0af576f)

   (Working)
3. check the traffics in Nekoray.
   ![2025-02-20_09-49-26](https://github.com/user-attachments/assets/6c076d0a-da4d-4842-a49f-9fd38c338f12)




## Android

### Requirements

[Byedpi-Neko plugin](https://github.com/hufrea/byedpi-neko).

[NekoBoxForAndroid](https://github.com/MatsuriDayo/NekoBoxForAndroid).

Download and install both.

### Steps :
1. Open Nekobox.
2. Go to Tools >>> Backup >>> Import from file (Import the custom settings I made).

   ![2025-02-20_10-11-51](https://github.com/user-attachments/assets/89c51148-ca9b-4bdb-9722-4f1bd75af68e)
   ![2025-02-20_10-12-14](https://github.com/user-attachments/assets/56b39fa6-39ff-4f76-b5f5-092609af1234)
   ![2025-02-20_10-12-39](https://github.com/user-attachments/assets/0e4bc22c-8880-4ea7-aca7-3fe0a7cc9071)
   ![2025-02-20_10-13-08](https://github.com/user-attachments/assets/61cee61f-666b-4c28-8c86-08acde8d4f31)
   ![2025-02-20_10-13-59](https://github.com/user-attachments/assets/fa390e97-b9c6-4f83-81bf-9bd0165988c0)
   ![2025-02-20_10-14-36](https://github.com/user-attachments/assets/980f4ab1-c070-49d6-a5cf-25aa36a1f08f)
   
3. Choose the desired profile and run it.
   
   ![2025-02-20_10-15-33](https://github.com/user-attachments/assets/c2e9c114-dd78-4626-88e8-59f6f39eb0c3)
   ![2025-02-20_10-16-11](https://github.com/user-attachments/assets/4897f9bf-f0d2-4cb3-a7bf-aae0414c89ce)

- the mentioned file is [Here](https://github.com/Therapist191124/LocalSOCKS5DPIBYPASS/releases/download/Custom_Setting/nekobox_backup_Feb.20.2025.10_01_51.AM.json)

### Add Custom profile :

Advanced plugin >>> Choose ByeDPI >>> Enable manual mode >>> Edit options :
![2025-02-20_11-46-29](https://github.com/user-attachments/assets/3c301877-ac72-4d3e-b124-a2cf9994b0e9)
![2025-02-20_11-47-08](https://github.com/user-attachments/assets/6fe0be7a-088f-461c-a2eb-40720d216a2b)
![2025-02-20_11-47-46](https://github.com/user-attachments/assets/451bab7d-a206-4e6c-90f1-7ddf2ba43fc7)
![2025-02-20_11-48-26](https://github.com/user-attachments/assets/11ef6171-c662-40ed-86dd-5d5db4b4872d)
![2025-02-20_11-48-51](https://github.com/user-attachments/assets/a96d1326-fdff-4f35-a87a-e21b54b8c1a3)
![2025-02-20_11-50-33](https://github.com/user-attachments/assets/ab728494-d7c4-40ff-914d-21b18428ec69)
![2025-02-20_11-51-10](https://github.com/user-attachments/assets/10d25b15-6cd2-4712-910a-89e95fbb9372)

```bash
--fake -2 --tls-sni Ea.com --tlsrec 6+s --tlsrec 27+s
```
- You can change "Ea.com" with the desired host you would like to use.

Replace the existing one with this parameter.

## Create custom parameter

```bash
-i, --ip  
    Listening IP, default is 0.0.0.0

-p, --port  
    Listening port, default is 1080

-D, --daemon
    Run in daemon mode
    Supported only on Linux and BSD systems

-w, --pidfile  
    PID file location

-E, --transparent
    Run in transparent proxy mode, SOCKS will not work
    
-c, --max-conn  
    Maximum number of client connections, default is 512

-I, --conn-ip  
    Address to which outgoing connections will be bound, default is ::
    If an IPv4 address is specified, IPv6 requests will be rejected

-b, --buf-size  
    Maximum size of data received and sent per recv/send call
    Size is specified in bytes, default is 16384

-g, --def-ttl  
    TTL value for all outgoing connections
    May be useful for bypassing detection of non-standard/reduced TTL

-N, --no-domain
    Drop requests if the address is a domain
    Since DNS resolution is performed synchronously, it may slow down or even freeze the operation

-U, --no-udp
    Do not proxy UDP
    
-F, --tfo
    Enable TCP Fast Open
    If the server supports it, the first packet will be sent immediately with SYN
    Supported only on Linux (4.11+)
    
-A, --auto  
    Automatic mode
    If an event similar to a block or failure occurs,
    then bypass parameters following this option will be applied
    Possible events:
         torst   : Timeout occurred or server dropped connection after the first request
        redirect: HTTP Redirect with Location whose domain does not match the outgoing one
         ssl_err : In response to ClientHello, ServerHello was not received or SH contains an incorrect session_id
        none    : The previous group was skipped, e.g., due to domain or protocol restrictions
    
-L, --auto-mode  
    0: Cache IP only if reconnection is possible
    1: Cache IP also in the case:
        torst - timeout/connection dropped during data exchange (i.e., after the first data from the server)
        ssl_err - only one round of data exchange occurred (request-response/request-response-request)
    
-u, --cache-ttl  
    Cache value lifetime, default is 100800 (28 hours)
    
-T, --timeout  
    Timeout waiting for the first response from the server in seconds
    On Linux, this is converted to milliseconds, so fractional numbers can be specified
    
-K, --proto  
    Protocol whitelist: tls,http,udp,ipv4
    
-H, --hosts  
    Limit the scope of parameters to a list of domains
    Domains should be separated by a newline or space
    
-j, --ipset  
    Restriction by specific IPs/subnets
    
-V, --pf  
    Port restriction
    
-R, --round  
    To which/which request to apply obfuscation
    Default is 1, i.e., to the first request
    
-s, --split  
    Split the request at the specified position
    Position has the form offset[:repeats:skip][+flag1[flag2]]
    Flags:
        +s: add SNI offset
        +h: add Host offset
        +n: zero offset
    Additional flags:
        +e: end; +m: middle
    Examples: 
        0+sm - split the request in the middle of SNI
        1:3:5 - split at positions 1, 6, and 11
    The key can be specified multiple times to split the request at several positions
    If the offset is negative and has no flags, the offset is added to the packet size
    
-d, --disorder  
    Similar to --split, but parts are sent in reverse order
    
-o, --oob  
    Similar to --split, but part is sent as OOB data
    
-q, --disoob  
    Similar to --disorder, but part is sent as OOB data
    
-f, --fake  
    Similar to --disorder, except before sending the first piece, a part of fake data is sent
    The number of bytes sent from the fake equals the size of the split part
    ! May be unstable on Windows
 
-t, --ttl  
    TTL for the fake packet, default is 8
    It is necessary to select a value such that the packet does not reach the server but is processed by DPI

-k, --ip-opt[=file|:str]
    Set options for the fake IP packet
    Significantly reduces the probability that the packet will reach the server
    Note that it may not reach the DPI either
    Not supported on Windows
    
-S, --md5sig
    Set the TCP MD5 Signature option for the fake packet
    Most servers (mainly on Linux) drop packets with this option
    Supported only on Linux, may be disabled in some kernel builds (< 3.9, Android)

-O, --fake-offset  
    Offset the start of fake data by n bytes
       
-l, --fake-data  
    Specify your own fake packets
    The string can contain escape characters (\n,\0,\0x10)

-e, --oob-data  
    Byte sent out-of-band, default is 'a'
    Can specify ASCII or escape character
    
-n, --tls-sni  
    Change the SNI in the default fake packet to the specified one

-M, --mod-http  
    Various manipulations with the HTTP packet, can be combined
    hcsmix:
        "Host: name" -> "hOsT: name"
    dcsmix:
        "Host: name" -> "Host: NaMe"
    rmspace:
        " Host: name" -> "Host:name\t"

-r, --tlsrec  
    Split ClientHello into separate records at the specified offset
    Can be specified multiple times  

-a, --udp-fake  
    Number of fake UDP packets

-Y, --drop-sack
    Ignore SACK, forcing the kernel to retransmit already delivered packets
    Supported only on Linux
```
## More Details

### `--split`
Splits the request into parts. Example on a 30-byte request:

- **Parameters:** `--split 3 --split 7`
- **Sending order:** 1-3, 3-7, 7-30  
Positions should be specified in ascending order.

---

### `--disorder`
The part falling under disorder will be sent with TTL=1, meaning it will not actually be delivered anywhere. The OS learns about this only after sending the subsequent part, when the server reports the loss using SACK. The system will have to resend the previous packet again, thereby disrupting the usual order.

- **Parameters:** `--disorder 7`
- **Sending order:** 7-30, 1-7  

**Note:** The above applies only to Linux.  
On Windows, retransmission starts from the position where the losses began (the maximum ACK received from the server):

- **Parameters:** `--disorder 7`
- **Sending order:** 7-30, 1-30  

Therefore, it is advisable to use `split` as well:

- **Parameters:** `--split 7 --disorder 23`
- **Sending order:** 1-7, 23-30, 7-30  

In practice, it's optimal to use:
- **Linux:** `--disorder 1`
- **Windows:** `--split 1+s --disorder 3+s`

---

### `--fake`
Data in the first part of the request is replaced with fake data. This part should pass through the DPI but not reach the server.

- **Parameters:** `--fake 7`
- **Sending order:** 1-7 fake, 7-30 original, 1-7 original  

To ensure the fake doesn't reach the server, there are options like `ttl`, `ip-opt`, and `md5sig`.  
TTL must be selected such that the packet passes through all DPI but does not reach the server. For Linux, there's `md5sig`. It sets the TCP MD5 Signature option, which prevents many servers from accepting the packet. Unfortunately, `md5sig` doesn't work in all builds.  

For Windows, there's another way to avoid server processing of the fake. This involves combining `fake` with `disorder`:

- **Parameters:** `--disorder 1 --fake 7`
- **Sending order:** 2-7 fake, 7-30 original, 1-30 original  

If the fake packet reaches the server, it will be overwritten due to full retransmission.  

In practice, it's optimal to use:
- **Linux:** `--fake -1 --md5sig`
- **Windows:** `--disorder 1 --fake -1`

---

### `--oob`
TCP can send data outside the main stream using the URG flag, but only 1 byte per packet. All data in such a packet will be delivered to the application, except the last byte, which is out-of-band.

- **Parameters:** `--oob 3`
- **Sending:** 1-4 with URG flag (1-3 request data + 4th byte, which will be truncated), 3-30  

This byte is preferably placed in the SNI: `--oob 3+s`

---

### `--disoob`
Similar to `--disorder`, but part is sent with an OOB byte.

- **Parameters:** `--disoob 3`
- **Sending:** 3-30, 1-4 with URG flag (1-3 + byte that will be truncated + 4-8)  

When used with `--fake` or `--disorder`, you can get a packet where the OOB byte is located at the split point:

- **Parameters:** `--disoob 3 --disorder 7`
- **Sending:** 3-30, 1-8 with URG flag (1-3 + byte that will be truncated + 4-8)

---

### `--tlsrec`
A single TLS record can be split into several, slightly modifying the header. At the split point, a new header is inserted, increasing the request size by 5 bytes.

This header can be placed in the middle of the SNI, preventing DPI from reading it correctly:

- **Parameters:** `--tlsrec 3+s`  

Although `tlsrec` and `oob` confuse DPI, they can also confuse various middleboxes that do not support a full TCP/TLS stack. Therefore, they should be used together with `--auto`:

- **Example:** `--auto=torst --timeout 3 --tlsrec 3+s`  
In this case, `tlsrec` will be applied only in cases where the connection is dropped or the timeout has been reached, i.e., when blocking likely occurred.  

You can do the opposite - cancel `tlsrec` if the server drops the connection or discards the packet:

- **Example:** `--tlsrec 3+s --auto=torst --timeout 3`

---

### `-Y, --drop-sack`
Causes the kernel to ignore packets with the TCP SACK extension. This extension allows acknowledgment of receipt of individual data segments.

If the first part of the request is lost and only the second part reaches the server, the server can notify the client of this using this extension. Then the client, knowing that the second part has arrived, will send only the first.  

Why ignore this extension? The second segment might be fake. If it reaches the server but the client does not know about it, the client will attempt to retransmit it. However, this segment will contain the original data, which will overwrite the fake, thereby preventing protocol disruption.  

Since fast acknowledgment won't work, this will break `disorder` and add delay before retransmission (about 200ms).

---

### `--auto`, `--hosts`
The `auto` parameter divides options into groups. For each request, they are traversed from left to right. First, the trigger specified in `auto` is checked, then `pf`, `proto`, and `hosts`.

You can specify multiple groups of options, separating them with this parameter. Parameters that come below `--timeout` in the help text (except `tls-sni`) can be moved into a separate group.
