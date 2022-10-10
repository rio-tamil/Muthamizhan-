
# Project Title



Classification of arrhythmia by using deep learning with 2-d ecg spectral image representation
## Team Lead
  A.Muthamizhan
## Team Member
  PL. Vetriselvan - member  1

  R. Bharathidasan - member 2
  
  R. Vignesh kumar - member 3
  
  name: Generate Datas
on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"
  workflow_dispatch:
jobs:
  build:
    name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Snake Animation
      - uses: Platane/snk@master
        id: snake-gif
with:
          github_user_name: thepiyushmalhotra
          svg_out_path: dist/github-contribution-grid-snake.svg
      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
