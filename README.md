---
note: generated by cobra
path: /cmd/docs.go
---
# kabanero CLI
## kabanero

This repo defines a command line interface used by the enterprise, solution, or application architect who defines and manages the kabanero collections that are used by developers to create governed applications for their business.

### Synopsis

**kabanero** is a command line interface for managing the collections in a Kabanero 
environment, as well as to on-board the people that will use 
the environment to build applications.

Complete documentation is available at https://kabanero.io

### Options

```
  -h, --help      help for kabanero
  -v, --verbose   Turns on debug output and logging to a file in $HOME/.kabanero/logs
```

### SEE ALSO

* [kabanero deactivate](#kabanero-deactivate)	 - Prevent this collection from being shown to the development team, while not deleting it.
* [kabanero list](#kabanero-list)	 - List all the collections in the kabanero instance, and their status
* [kabanero login](#kabanero-login)	 - Will authentic you to a Kabanero instance
* [kabanero logout](#kabanero-logout)	 - Disconnect from Kabanero instance
* [kabanero onboard](#kabanero-onboard)	 - Command to onbboard a developer to the Kabanero infrastructure
* [kabanero refresh](#kabanero-refresh)	 - Refresh the collections list
* [kabanero version](#kabanero-version)	 - Show Kabanero CLI version

###### Auto generated by spf13/cobra on 28-Aug-2019
## kabanero login

Will authentic you to a Kabanero instance

### Synopsis


	Login to a Kabanero instance using github credentials, and store a temporary access token for subsequent command line calls.
	The temporary authentication token will be stored in your-home-directory/.kabanero/config.yaml.
	Use your github userid and either password or Personal Access Token (PAT).
	

```
kabanero login userid Github-PAT|Github-password kabanero-url [flags]
```

### Examples

```

	# login with Github userid and password:
	kabanero myGithubID myGithubPassword https://my.kabaneroInstance.io

	# login with Github userid and PAT:
	kabanero myGithubID myGithubPAT https://my.kabaneroInstance.io
	
```

### Options

```
  -h, --help   help for login
```

### Options inherited from parent commands

```
  -v, --verbose   Turns on debug output and logging to a file in $HOME/.kabanero/logs
```

### SEE ALSO

* [kabanero](#kabanero)	 - This repo defines a command line interface used by the enterprise, solution, or application architect who defines and manages the kabanero collections that are used by developers to create governed applications for their business.

###### Auto generated by spf13/cobra on 28-Aug-2019
## kabanero logout

Disconnect from Kabanero instance

### Synopsis


Disconnect from the instance of Kabanero that you 
have been interacting with.

```
kabanero logout [flags]
```

### Options

```
  -h, --help   help for logout
```

### Options inherited from parent commands

```
  -v, --verbose   Turns on debug output and logging to a file in $HOME/.kabanero/logs
```

### SEE ALSO

* [kabanero](#kabanero)	 - This repo defines a command line interface used by the enterprise, solution, or application architect who defines and manages the kabanero collections that are used by developers to create governed applications for their business.

###### Auto generated by spf13/cobra on 28-Aug-2019
## kabanero list

List all the collections in the kabanero instance, and their status

### Synopsis

List all the collections in the kabanero instance, and their status

```
kabanero list [status] [flags]
```

### Options

```
  -h, --help   help for list
```

### Options inherited from parent commands

```
  -v, --verbose   Turns on debug output and logging to a file in $HOME/.kabanero/logs
```

### SEE ALSO

* [kabanero](#kabanero)	 - This repo defines a command line interface used by the enterprise, solution, or application architect who defines and manages the kabanero collections that are used by developers to create governed applications for their business.

###### Auto generated by spf13/cobra on 28-Aug-2019
## kabanero refresh

Refresh the collections list

### Synopsis

Refresh reconciles the list of collections from master to make them current with the activated collections across all namespace in the kabanero instance

```
kabanero refresh [flags]
```

### Options

```
  -h, --help   help for refresh
```

### Options inherited from parent commands

```
  -v, --verbose   Turns on debug output and logging to a file in $HOME/.kabanero/logs
```

### SEE ALSO

* [kabanero](#kabanero)	 - This repo defines a command line interface used by the enterprise, solution, or application architect who defines and manages the kabanero collections that are used by developers to create governed applications for their business.

###### Auto generated by spf13/cobra on 28-Aug-2019
## kabanero onboard

Command to onbboard a developer to the Kabanero infrastructure

### Synopsis

Under development.  In the future this command causes an email to be sent to the user associated
	with the user-id providing the information necessary to get started using 
	Kabanero.

```
kabanero onboard github-id repo-name [flags]
```

### Options

```
  -h, --help   help for onboard
```

### Options inherited from parent commands

```
  -v, --verbose   Turns on debug output and logging to a file in $HOME/.kabanero/logs
```

### SEE ALSO

* [kabanero](#kabanero)	 - This repo defines a command line interface used by the enterprise, solution, or application architect who defines and manages the kabanero collections that are used by developers to create governed applications for their business.

###### Auto generated by spf13/cobra on 28-Aug-2019
## kabanero deactivate

Prevent this collection from being shown to the development team, while not deleting it.

### Synopsis


A collection can be available to a development team
to use for building applications or not. deactivate
will cause the collection to not be shown to 
the develoopment team when they list the types of
application they can build.

This would be done in the case where you have cloned the collection
and made changes for your business.  This keeps the base collection
in the apphub, and it will continue to be updated, and the 
updates will be perkolated up to your cloned collection.

```
kabanero deactivate collection-name [flags]
```

### Options

```
  -h, --help   help for deactivate
```

### Options inherited from parent commands

```
  -v, --verbose   Turns on debug output and logging to a file in $HOME/.kabanero/logs
```

### SEE ALSO

* [kabanero](#kabanero)	 - This repo defines a command line interface used by the enterprise, solution, or application architect who defines and manages the kabanero collections that are used by developers to create governed applications for their business.

###### Auto generated by spf13/cobra on 28-Aug-2019
