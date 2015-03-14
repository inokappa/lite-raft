lite-raft implement the Raft consensus algorithm and want to be 100% compliant with the specification.
I try to write portable code with POSIX standards or commands widely supported.
For now runs without syntax error on Linux, HP-UX and OpenBSD.

Current status:
replication, leader election, a simple client to set/get values, test-and-set,
cluster membership change, log snapshotting, portability fix.
Runs on Linux and HP-UX, to be tested soon OpenBSD.
You can even have mixed OS in the raft cluster! this feature is not a priority
but a consequence of the portability patches :)

The module that implement a failover cluster has been moved to a new project, see:
> https://code.google.com/p/back-to-work/
and its required distributed lock manager:
> https://code.google.com/p/dex-lock/


---


take a look at the raft algorithm: http://raftconsensus.github.io

Mail me at: luigi |dot| tarenga |at| gmail |dot| com