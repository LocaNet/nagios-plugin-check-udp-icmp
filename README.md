nagios-plugin-check-udp-icmp
============================

Overview:

	Nagios plugin to check if a UDP port connection attempt returns an ICMP message
	or not.

Usage:

	$USER1$/check_udp_icmp [-H <host>] [-p <port>]

	The script will return OK if a ICMP message is being received and CRITICAL if
	no ICMP response arrives after 10 seconds.

	Please note that root privileges are required to create the raw socket that
	will receive the ICMP packets.

Requirements:

	The script requires the Monitoring::Plugin Perl module.
