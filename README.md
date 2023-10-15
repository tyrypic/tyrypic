- uses: Platane/snk@v3
  with:
    github_user_name: ${{ github.tyrypic }}

    outputs: |
      dist/github-snake.svg
      dist/github-snake-dark.svg?palette=github-dark
      dist/ocean.gif?color_snake=orange&color_dots=#bfd6f6,#8dbdff,#64a1f4,#4b91f1,#3c7dd9

  env:
    GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
