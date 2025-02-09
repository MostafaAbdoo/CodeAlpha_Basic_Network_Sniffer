# CodeAlpha_Basic_Network_Sniffer
a basic network sniffer program using python
# Explanation

    packet_callback Function:
        This function processes each captured packet.
        It checks if the packet has an IP layer.
        It extracts the protocol number, source IP, and destination IP from the IP layer.
        It determines the protocol name based on the protocol number.
        It prints the protocol name, source IP, and destination IP.
    main Function:
        This function starts capturing packets on the default network interface.
        The ‘sniff‘ function is called with ‘prn=packet_callback‘ to specify the callback function for each captured packet, filter=”ip” to capture only IP packets, and ‘store=0‘ to avoid storing packets in memory.
