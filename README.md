About
===========

Integrate the C testing harness [Unity](http://throwtheswitch.org/white-papers/unity-intro.html) in the wink of an eye.

Getting started
-----------------

Clone the repository and run:

```bash
	# download and extract unity source
	make bootstrap

	# create two test files/groups
	make new name=foo
	make new name=bar

	# run all test files/groups
	make

	# run only test group `foo`
	make TESTS=foo
```


* Change `OPEN_IN_EDITOR` from **true** to your editor e.g **vim** to
open a test file/group automatically with `make new name=<name>`

* The template for `make new` is `bin/group.c.template`
* The template for the test runner is generated by  `bin/assemble_groups.sh`