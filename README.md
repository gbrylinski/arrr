# Creation miracle

this small set of *Ansible* roles have been created as a result of presentation I prepared some time ago. It proofs or rather should proof ideas I proposed to make shared roles cleaner and easier to (re)use.

Ideas behind the roles come mostly from my experiences and knowledge found on the net. Not especially new stuff, just put together and structured a bit.

# Ideas

The base principles I tried to keep to are as follows:

- role should be as simple as possible
- one role, one responsibility. Multiple simple roles are better than single uber-mega-do-everything-yeah role
- no shared top level variables except some really, really global like e.g. `stage`
- every role's variables are prefixed with a role name or packed into a hash named after the role
- each role has a short README telling what it does and how

# Requirements

- **Ansible** of course is rather necessary - [how to install](http://docs.ansible.com/ansible/intro_installation.html)

# More roles?

This is a work-in-progress so more roles come soon. Stay tuned (-;
