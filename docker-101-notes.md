# Docker 101 Presentation Notes

* https://12factor.net/
* roland [12:53 PM]
	* I think it was related to 12 factor, and the ephemeral nature of the containers; so things like 
		- don't expect to write things to disk and expect them to be there later, write it to  a volume
		- don't bake configurations into the image
		- treat them as disposable; if a container is failing somehow, just kill it and restart another
		- have the code expect to be stateless