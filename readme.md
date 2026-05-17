# Website is live at

https://avadae.github.io/game-groupprojects/

# Instalation (windows)

In an elevated terminal:

```
winget install --force RubyInstallerTeam.RubyWithDevKit.3.4
bundle install
```

# Run the website (windows)

```
bundle exec jekyll server --livereload -s ./src
```

# Command to convert jpg and png to webp

```
Get-ChildItem -Path ./* -Include *.jpg, *.png -File | ForEach-Object { cwebp -q 75 $_.FullName -o "$($_.Directory)\$($_.BaseName).webp" }
```