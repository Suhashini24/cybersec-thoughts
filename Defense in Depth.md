# Is Defense in Depth still relevant?

Defense in depth has long been a topic graduates and organizations have followed. In day-to-day terms, defense in depth is basically the act of building a fence around your land, then a gate with a lock at the edge, a door with a different lock (like a key pad) at the entrance of your home, having strong walls, windows that are not easily reachable by an average human, iron grills fitted behind the windows that can be accessed by anyone outside, different doors with individual locks to different rooms, having CCTV, or perhaps, if you have important stuff in your home, even having a dog or a security guard. 

Similarly, in traditional on-premises environments, the “fence” has always been a firewall and the different doors are always other “internal firewalls” or sometimes VLANs configured in switches. Endpoint protection software act as the lock to your money vault or cupboard (where your clothes and jewelry are stored). Log monitoring has always acted as the CCTV where the SIEM is always “logically”, sometimes physically segregated (in another location – could be a managed security service provider). 
But is it the same in the cloud? Now that it has pretty much become a one-stop-shop for all needs.

Keeping aside regulatory requirements that need to be adhered to (sometimes resulting in opting out of the cloud), any architecture still needs defense in depth. This is why there is a “**shared responsibility model**” in the cloud. 
#### The cloud service provider will own and handle 
* The physical security of the data centers hosting the servers that run the hypervisors on top of which client applications, services and data are run and stored.
* Patching and vulnerability management of the server operating system and hypervisor.
*	Access control of who can access the servers (physically) and who can configure server configurations.
#### The client (i.e. you and I) will own:
*	The protection of the application and environment created on the virtualized environment run on top of the hypervisors. 

So, what does “**_The protection of the application and environment created on the virtualized environment run on top of the hypervisors_**” mean?

I will explain my view on how a system must generally be designed, irrespective of data criticality. Then I will suggest further controls for critical system or regulated systems.

# Version Control
24/09/2025 - Initial draft
