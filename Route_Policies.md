Discuss Policy-based routing
create a static route policy

Services and Interfaces are used to configure static routes to forward traffic

Creating route policy:
1. Policy > Rules and Policies > Routing Rules > Add
2. Specify Name, Tags, and Description
3. Change Lookup source with dropdown arrow
4. Change Service Object with dropdown arrow
5. Next Hop
	1. Multi-path route: Use routes of equal cost
	2. SD-WAN Rule
	3. Standard Route is default
	4. Select interface with Interface dropdown
	5. Gateway is set to 0.0.0.0/:: by default
	6. Metric can be set between 0 and 255
	7. Lower metric = higher priority
6. Advanced
	1. Static routes take precedence over VPN tunnels unless 'Allow VPN path to take precedence' is enabled
	2. TOS (Type of Service) routing Value and Mask bit compare to inbound packet values to find a match and apply to packets entering the firewall. Default value is 0. Routes with higher TOS values are given precedence. 
7. Probe
	1. Used to create a network monitor object