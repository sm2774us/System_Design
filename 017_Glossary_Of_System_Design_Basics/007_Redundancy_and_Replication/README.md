# Redundancy and Replication
-------------------------------------------------

[Redundancy](https://en.wikipedia.org/wiki/Redundancy_(engineering)) is the duplication of critical components or functions of a system with the intention of increasing 
the reliability of the system, usually in the form of a backup or fail-safe, or to improve actual system 
performance. For example, if there is only one copy of a file stored on a single server, then losing that server 
means losing the file. Since losing data is seldom a good thing, we can create duplicate or redundant copies of 
the file to solve this problem.

Redundancy plays a key role in removing the single points of failure in the system and provides backups if 
needed in a crisis. For example, if we have two instances of a service running in production and one fails, the 
system can failover to the other one.

![redundancy_and_replication](assets/redundancy_and_replication.PNG)

[Replication](https://en.wikipedia.org/wiki/Replication_(computing)) means sharing information to ensure consistency between redundant resources, such as software 
or hardware components, to improve reliability, [fault-tolerance](https://en.wikipedia.org/wiki/Fault_tolerance), or accessibility.

Replication is widely used in many database management systems (DBMS), usually with a primary-replica 
relationship between the original and the copies. The primary server gets all the updates, which then ripple 
through to the replica servers. Each replica outputs a message stating that it has received the update 
successfully, thus allowing the sending of subsequent updates.

:back:[**Back - Proxies**](../006_Proxies/README.md)
:arrow_right:[**Next - SQL vs. NoSQL**](../008_SQL_vs_NoSQL/README.md)

### Progress Tracker

- [x] Mark as Completed
