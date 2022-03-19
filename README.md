# mypackage

we are in directory d

- to create a node package
  - choose a <name> for you package
    - see naming conventions
  - mkdir <name>
  - cd <name>
  - create git repo
    - add Readme.md, .gitignore, .npmignore files
    - git init
    - git add --all
    - git commit -m "initial commit name"
    - git remote add origin git@github.com:username/name.git
  - create package structure
    - npm init
      - name
      - version
      - it will pick up git uri
      - main (index.js)
    - Add You Code
      - the main (index.js) will be loaded when require is invoked
    - Let local system know about the package
      - npm link
- test package locally
  - cd .. (d), 
    - mkdir test, cd test, add testme.js
      - edit testme.js add require('name')
      - npm link name
      - will add name package under modules
- Publish to npm repository
  - npm login
    - username/pass then OTP