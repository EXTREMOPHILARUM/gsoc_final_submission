# GSoC 2021 OWASP OWTF - General Improvements

Hello everyone,
I am Saurabh, a final year student Computer engineering at NIT Kurukshetra. I would like to thank the OWASP organization for giving me this opportunity to work on the OWASP OWTF project with GSoC.


## About my project:
My project was about imporoving the stability of the framework along with adding the new features to the framework. In the course of the 10 weeks I worked on migrating the CI jobs from travis to github actions. Implementing a new feature that can help you to create custom plugin groups. Improved the speed of the fronted by implementing react lazy loading.

## Work done

### Migrating from Travis CI to Github Actions
Travis CI eneded their free plan for communities resulting in the the CI pipelines for OWTF to stop. This was fixed by migrating it to Github Actions.
<br>Fix: [link](https://github.com/owtf/owtf/pull/1150/)

### Custom test groups feature
The default plugin groups allow the user to execute three basic categories of plugins this PR imporves that functionality by allowing the user to create custom groups right from the frontend.
<br>Fix: [link](https://github.com/owtf/owtf/pull/1154/)

### Implement React lazy loading and Upgrade to webpack 4
A website experience is defined by how smooth it can function and how fast it can function also this is a step forward in upgrading the project with the latest dependencies.
<br>Fix: [link](https://github.com/owtf/owtf/pull/1164)

### Fixed Logs not showing up on the workers and Dashboard page
Clicking on the button to show logs resulted in an error.
<br>Fix: [link](https://github.com/owtf/owtf/pull/1098/)

### Update OWTF install script and add documentations
The makefile being used to install the framework had elements that were not working and the documentations for the installations were not being proper according to the updated scripts.
<br>Fix: [link](https://github.com/owtf/owtf/pull/1145)

### Web UI stuck on loading application
The web interface is stuck on loading application as the latest version of node is not compatible with the npm packages.
<br>Fix: [link](https://github.com/owtf/owtf/pull/1135/)

### Fix yaml warning
The PyYaml library gave warning on using yaml.load and asked us to use yaml.safe_load. This PR aims to solve that.
<br>Fix: [link](https://github.com/owtf/owtf/pull/1165/)

### Fix too many clients error
The Async nature of the framework resulted in the system creating too many parallel connections with the db this resulted in the db to stop responding to the application until the pool is cleaned up.
<br>Fix: [link](https://github.com/owtf/owtf/pull/1166/)

## Future Work
After the completition of my GSoC goals I would keep working on updating the complete project codebase to support the latest dependencies and code styles so that we can again create a stable release of OWTF.

## Conclusion
To begin with I would like to than my mentors for being supportive and helping me with my project by providing me with the resources. I would also like to thank my fellow GSoC partner Aman for helping me in the project and also for solving my doubts. GSoC has helped me in getting started with open-source contributions. Although GSoC is coming to an end this I would still continue working on the project and many more in the coming future.

