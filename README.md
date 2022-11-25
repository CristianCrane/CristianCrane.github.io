## Running the jekyll site locally

### Dependencies
- VS Code
- VS Code Extension: `Dev Containers`
- Docker desktop

### Set up local environment
1. Start up your local container
    - Run `>Open Folder in Container` in VS code cmd prompt
    - specify the Dockfile if asked
    - open a terminal in VS code, it should be remotely connected to the container 
2. Install ruby dependencies required by jekyll
    - Run `bundle install` from your remote terminal
    - Run `bundle update`
    - this will install all the ruby dependencies specified in the `Gemfile.lock` file
3. Spin up local jekyll server
    - Run `bundle exec jekyll serve --livereload`
    - The jekyll site should now be available at port 4000

### Tear down local environment
1. Shut down the local jekyll server if you have it running
2. Stop the container
    - Run `>Remote: Close Remote Connection` in VS code cmd prompt
