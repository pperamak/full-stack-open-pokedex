Assuming that we have a team building an application using python, the probably best linter is pylint. I can be quite a process to set it up and configure it, but for a bigger project like this it is definitely worth it.

For testing the best option is probably pytest. It is simpler than most other testing frameworks, but also very powerful. It supports a wide ecosystem of plugins and extensions, so it is usable in many kind of python projects.

For the build step, python applications are usually packaged into wheels (.whl) or source distributions (.tar.gz). For this the standard tool is setuptools. If containerization is needed, Docker is used for packaging apps into containers.

For automating the entire continuous integration and build process, there are alternatives to GitHub Actions and Jenkins. These alternatives include GitLab CI/CD, Travis CI and CircleCI.

For a small team like this working on a single project, I think a cloud-based solution for CI would be best. The self-hosted options are quite complicated to set up, and we do not want to use too much of our team’s working time for that. For a small team working on a single app, a cloud-based solution like GitHub Actions is very good, since the configuration is simpler.