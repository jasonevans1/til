# Run a bash script from a Jenkinsfile in a Jenkins Pipeline

In order to run a bash script from within a Jenkinsfile (Groovy script) in a Jenkins pipeline you need to do the following. Make sure the she-bang line is the first line of the script.

```
sh '''#!/bin/bash -l
      cap alpha deploy
   '''
```

[source](http://stackoverflow.com/questions/35343948/how-can-i-start-a-bash-login-shell-in-jenkins-pipeline-formerly-known-as-workfl)
