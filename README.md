Updating autodoc.sh
===================

Remember to update the Makefile when re-creating the
sphinx documentation style.

Here are the needed steps:

1. TeX has to have the following packages installed:
   - `tlmgr install fancybox framed threeparttable mdwtools wrapfig parskip upquote`
2. Run `docs/autodoc.sh` for creating the documentation,
   This will automatically created and commit the documentation
   of the latest tag on the `master` branch.

	To skip the actual commit of the documentation call it via
	`docs/autodoc.sh --skip-commit|-sc`

To produce the documentation from a specific tag do:

    docs/autodoc.sh --tag <tag>
