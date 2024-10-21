# Compile ARM version

```shell
brew install mpv ffmpeg node cmake qt@5

brew install --cask qt-creator

git submodule update --init --recursive

brew install openssl

brew link openssl --force

brew link qt5 --force

qmake CONFIG+=sdk_no_version_check

cmake -DCMAKE_PREFIX_PATH=/opt/homebrew/opt/qt@5 .

cmake --build .

sh ./mac/finalize.sh

sh ./mac/pack.sh

```
