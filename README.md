# Site Seeker - Library

## Setup
Add to package.json
```
"siteseekerlib": "git+https://github.com/siteseeker-co/siteseekerlib.git#v1.0.0",
```
## Commands
Add the following to your package.json scripts
```  "scripts": {
"organize": "node node_modules/jscodeshift/bin/jscodeshift.js packages  --extensions=tsx,ts --parser=tsx -t node_modules/siteseekerlib/tools/organize.ts",
"test.deps": "yarn depcheck --ignores=depcheck,typescript,react-native-web",
},
```