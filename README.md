# toolarium-common-gradle-build-config
Defines the toolarium organization common-gradle-build configuration definitions.

This repository was created by the cb:
1) cb --new
2) choose option "Common Organization Config"
3) Init git repository and pushed to the repository
4) Set project reference in configuration in gradle\defaults.gradle
```
setCommonGradleProperty("commonGradleBuildHomeGitUrl", "https://github.com/toolarium/toolarium-common-gradle-build-config.git")
setCommonGradleProperty("commonGradleBuildHomeVersionFileUrl", "https://raw.githubusercontent.com/toolarium/toolarium-common-gradle-build-config/master/VERSION")
setCommonGradleProperty("commonGradleBuildCustomConfigName", "Toolarium Config")
```
5) Set generell project license in configuration in gradle\defaults.gradle
```
setCommonGradleProperty("licenseOrganisation", "toolarium")
setCommonGradleProperty("licenseText", "")
setCommonGradleProperty("licenseUrl", "https://github.com/toolarium")
```
6) Added on local machine the configuration reference. Created the path and a file .cb-custom-config with the content `https://github.com/toolarium/toolarium-common-gradle-build-config.git`
   - Windows: %USERPROFILE%\.common-build\conf\.cb-custom-config
   - Linux: $HOME/.common-build/conf/.cb-custom-config
7) Called `cb --update`

After this steps your local cb / common build follows the guidelines of the git repository toolarium-common-gradle-build-config.
