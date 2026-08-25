# Resilient WAN Failover Architecture — Dual-Site Enterprise Network with Automated Backup Routing

Link to the Project videos on YT: https://www.youtube.com/playlist?list=PLbDbgJU7PWKA

This project extends a previously built dual-site enterprise network for TechCorp by adding a second, independent WAN path between its two buildings, removing the single point of failure created by relying on one fibre circuit alone. Using Cisco Packet Tracer, a backup ADSL link was provisioned alongside the existing primary fibre connection, with floating static routes configured so the backup path remains invisible in the routing table until it is actually needed.

To make the failover genuinely automatic rather than dependent on manual reconfiguration, the project also implements dynamic failure detection so that traffic reroutes onto the backup path within seconds of the primary link going down, and reverts automatically once the primary link recovers. The design was validated through deliberate, controlled failure testing: the primary link was physically removed to simulate a real outage, connectivity was confirmed to continue uninterrupted over the backup path, and the network was shown to heal itself once the primary path was restored.

The result is a self-healing network topology that mirrors how real enterprise WAN redundancy is designed and tested in production environments, with full evidence captured at every stage — from initial provisioning through to failure simulation and recovery confirmation.
