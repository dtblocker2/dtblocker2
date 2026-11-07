name: Draw Git Koi

on:
  schedule:
    - cron: '0 0 * * *' # Runs daily
  workflow_dispatch:

permissions:
  contents: write

jobs:
  koi:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout repository
        uses: actions/checkout@v4

      - name: Run git-profile-koi
        uses: yalongwastaken/git-profile-koi@v1
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
