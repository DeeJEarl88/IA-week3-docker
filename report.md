# Docker Security Homework

## Source Material
[Securing Docker - 6 best practices](https://vulcan.io/blog/securing-docker-ultimate-guide)

## Summary
Docker has become a popular and highly utilized software in the past several years. Its high adoption rate as a development and production tool has made it an attack vector to monitor and maintain. In reading this article it becomes apparent there's several areas in which docker software can be taken advantage of.

Areas of docker that pose security concerns, if not properly handled, include docker image composition, network constraints, and access controls. Developer should use software composition analysis tools to analyze image dependencies risks and remediate before attacks can exploit. It is also wise to implement container constraints on memory in the instance a container does become compromised to minimize fallout. Lastly, developers should ensure their containers are running with only the permissions necessary to do it's job. Always avoid running in root!


## Key Takeaways
- Ensure all containers are deployed and run with minimal privileges. This might look like a running process periodically validating containers or even a pipeline check to ensure new containers meet conditions before allowing traffic through.
- I never thought to apply resource constraints on containers but seems like  reasonable thing to add and reduce


## Questions
- Was the security practice or vulnerability you researched particular to Docker, or not?
  + There were several topics covered all of which are specific to Docker.

- Was the security practice or vulnerability related to the core docker system itself, the extended environment (e.g. Docker Hub), or Docker images (a.k.a. the software inside the Docker image)?
  + The security practices included both the core docker system as well as docker images

- Is this something that you should be concerned about within your particular company?
  + I feel pretty confident that Nationwide has safe guard in place to ensure several of these practices are followed and enforced.