# code build

- **codebuild** is a fully-managed **build pipeline** to create temporary servers to build and test code
- compile source code, run unit tests, and produce artifacts that are ready to deploy
- provide prepackaged build environments or you can build your own environments as a Docker container
- uses a buildspec.yml to provide build instructions. this file is stored in the root of your project.
  - version 0.1 - runs each build command in a separate instance
  - version 0.2 - runs all build commands in the same instance
  - commands run through different **phases:**
    - **install** only for installing packages in the build env
    - **pre_build** commands that run before building
    - **build** commands that you run during the build
    - **post_build** commands run after the build
  
