#2.1.3 (July 6th, 2014)
###Bug fixes:
- merging [pull request #4](https://github.com/jenkinsci/parameterized-remote-trigger-plugin/pull/4)


#2.1.2 (April 26th, 2014)
###Bug fixes:
- fixing [JENKINS-22325](https://issues.jenkins-ci.org/browse/JENKINS-22325) - local job fails when not sending any parameters to remote job
- fixing [JENKINS-21470](https://issues.jenkins-ci.org/browse/JENKINS-21470) - UI does not display that a build is using a file to get the parameter list
- fixing [JENKINS-22493](https://issues.jenkins-ci.org/browse/JENKINS-22493) - 400 when remote job has default parameters and parameters are not explicitly list them
- fixing [JENKINS-22427](https://issues.jenkins-ci.org/browse/JENKINS-22427) - fails when remote job waits for available executor


#2.1 (Feb 17th, 2014)
###New Feature/Enhancement:
- ability to specify the list of remote parameters from a file ([request ticket](https://issues.jenkins-ci.org/browse/JENKINS-21470))
- optionally block the local build until remote build is complete ([request ticket](https://issues.jenkins-ci.org/browse/JENKINS-20828))

###Misc:
- the console output has also been cleansed of displaying any URLs, since this could pose a security risk for public CI environemnts. 
- special thanks to [@tombrown5](https://github.com/timbrown5) for his contributions to the last item mentioned above


#2.0 ( Dec 25th, 2013)

Lots of refactoring and addition of some major new features.

###New Feature/Enhancement:
- integration with the 'Credentials' plugin ([request ticket](https://issues.jenkins-ci.org/browse/JENKINS-20826))
- able to override global credentials at a job-level ([request ticket](https://issues.jenkins-ci.org/browse/JENKINS-20829))
- support for 'Token Macro' plugin ([request ticket](https://issues.jenkins-ci.org/browse/JENKINS-20827))
- support for traditional Jenkins environment variables ([request ticket](https://issues.jenkins-ci.org/browse/JENKINS-21125))

###Misc:
Special thanks to [@elksson](https://github.com/elksson) for his contributions to the last 2 items mentioned above and to [@imod](https://github.com/imod) for his awesome feedback and feature suggestions.


#1.1 ( Nov. 30th, 2013)

###Bug fixes:
- closing potential security gap for public-read environments
    
    
###New Feature/Enhancement:
- ability to not mark the build as failed if the remote build fails
    
    
###Misc:
- General code clean-up


#1.0 
Initial release

###Available features:
- Trigger parameterized build on a remote Jenkins server
- Trigger non-parameterized build on a remote Jenkins server
- Authentication via username + API token
- Support for "build token root" plugin
