## Containers
- Standardised unit of software.
- Package of code than contains the dependencies to run the code.
- The same containers always yield same results, no matter where the code is executed. (Avoids WOMP).
- Docker is the tool used to build and interact with these containers.

## Why Containers (Why independent standardised 'application packages')?
- Often have different production, test, and development environments.
- Issues can arise if people use different package/language/etc versions.
- Even personal projects, is one is run on node12 vs. node14 could require uninstalling and installing 'correct' package when working on each one.
- If containerised, all these issues are squashed.

- Much smaller and more efficient that creating a set of VMs on a single machine.
- Only containerise key requirements, native OS and hardware does the heavy lifting.