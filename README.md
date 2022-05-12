# UCB AutoPush
Auto push build results to github from Unity Cloud Build

![](https://i.imgur.com/dXWtCgL.png)

## Features
- Automatically push UCB build result to the selected github repo
- Sync version code at every build
- Compatible with all target platform on UCB

## Setting up
### Copy files to your project 
- Copy all files under `Assets/Editor/UCB/` (Please keep them at the same path)

### Configure Unity Cloud Build
- Config > (Build Target) > Advanced Option 
    - **Pre-Export Method Name** = `UCB_Script.PreExport`
- Config > (Build Target) > Enviroment Variables
    - **GITHUB_NAME** = Your github username
    - **GITHUB_MAIL** = Your github account
    - **GITHUB_PSW** = You github access token (require `repo` access, you can generate from here: https://github.com/settings/tokens)
    - **GITHUB_REPO** = The target repo you wanna push to

![](https://i.imgur.com/dte6hxW.png)

![](https://i.imgur.com/M3UUy0A.png)



### References
tekminewe/unity-cloud-build-auto-build-number
https://github.com/tekminewe/unity-cloud-build-auto-build-number


Uploading to Steam via Post Build Script - Unity Fourm  
https://forum.unity.com/threads/uploading-to-steam-via-post-build-script.1032253/#post-8024819


unity cloud build Post-Build Script upload to github pages
https://stackoverflow.com/questions/60791806/unity-cloud-build-post-build-script-upload-to-github-pages

