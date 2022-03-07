# project-default-template


github actions: 

name: Create repository visualizer diagram
on:
  push
jobs:
  get_data:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout code
        uses: actions/checkout@master
      - name: Update diagram
        uses: githubocto/repo-visualizer@0.7.1
        with:
          excluded_paths: "ignore,.github"
          
![Visualization of the repository visualizer diagram](./diagram.svg)


