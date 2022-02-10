## HOW TO PUBLISH


Add a .npmrc to your project, in the same directory as your package.json
```
registry=https://pkgs.dev.azure.com/SpringGlobal/_packaging/SpringGlobal/npm/registry/ 
                        
always-auth=true
```

Then, run vsts-npm-auth to get an Azure Artifacts token added to your user-level .npmrc file

```
vsts-npm-auth -config .npmrc
```

Note: You don't need to do this every time. npm will give you a 401 Unauthorized error when you need to run it again.

Having issues? See the instructions for using a Personal Access Token to authenticate.
https://dev.azure.com/SpringGlobal/mSeries%20React%20Shared%20Packages%20(Includes%20RN)/_packaging?_a=connect&feed=SpringGlobal


