# Description
Darknet is a term used to describe a portion of IP addresses that are purposefully unused in a networking system. Because this portion of the network is supposedly unused there should not be any traffic back and forth. By monitoring this section, we can use it as a trap to detect potential probs searching for open IPs and ports that can be used to attack the system such as a DDoS attack. 

This program takes a Pcap file that has been monitoring a darknet trap on a network system and analyses it for potential probs.  
- Proven to parse through 96,000,000 data packets (6.45 GB) in 6 minutes.

### Probe Types Scanned For:
- Horizontal
- Vertical
- Strobe

# Instillation
1.	Download repository and place inside your projects folder for your complier (Visual studio recommended).
2.	Download the sample [pcap file](https://drive.google.com/open?id=1jWuCKoDL5kHzjsJhS9TyHVh4abY_fflo "Google Drive") (contailing 2 million data packets).
3.	Place this pcap file within the “Network” folder.

    - If using your own pcap file, remember to format the file as libcap. You can do this by using "editcap" in comand line. This comes with wireshark.

            editcap -F libpcap <filename> <newFileName>(.pcap)

4.	Open the project, build and run it.

# UI
After the file is uploaded you are able to:
- View all suspect IP address
- Query the suspect IPs for a spcefic IP address
- Filter the suspect IPs by a specific probe type
