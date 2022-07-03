# Inštalácia python
## pre Windows OS
> TBD
## pre Mac OS
Otvoríme si Terminal.

Nainštalujeme Brew spustením príkazu:
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> /Users/nikoleta.kocurova/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```
Nainštalujeme python spustením príkazu:
```
brew install python@3.9
```
Overíme Python verziu 3.9.13 spustením príkazu:
```
python3 --version
```
Ak tam je verzia 3.8 je potrebné ešte spustiť:
```
brew unlink python@3.9
brew unlink python@3.8
brew link --force python@3.9
```
# Inštalácia virtuálneho prostredia
## pre Windows OS
> TBD
## pre Mac OS
Nainštalujeme virtuálne prostredie spustním príkazu:
```
brew install pipenv
```
Overíme verziu virtuálneho prostredia spustením príkazu:
```
pipenv --version
```
Python 3.9 by mal byť nainštalovaný tu: /opt/homebrew/bin/python3.

Overíme to spustením príkazu:
```
which python3
```