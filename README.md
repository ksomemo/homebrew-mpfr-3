# homebrew-mpfr-3
for libmpfr4 (mpfr-3.1.6)

## install and settings
```bash
# for libmpfr6 (mpfr-4.x)
brew install mpfr
# => /usr/local/opt/mpfr/lib/libmpfr.6.dylib

# install mpfr3
brew unlink mpfr
brew install https://raw.githubusercontent.com/ksomemo/homebrew-mpfr-3/2c42cad41a1b36eec1f2b003575c6d9c13c6b652/Formula/mpfr.rb
# => /usr/local/Cellar/mpfr/3.1.6/lib/libmpfr.4.dylib

# setting for 4
brew unlink mpfr
ln -s /usr/local/Cellar/mpfr/4.0.1 /usr/local/opt/mpfr
brew link mpfr

# setting for 3
ln -s /usr/local/Cellar/mpfr/3.1.6/lib/libmpfr.4.dylib /usr/local/opt/mpfr/lib/libmpfr.4.dylib
```
