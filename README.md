## Pyppeteer
https://stackoverflow.com/questions/57217924/pyppeteer-errors-browsererror-browser-closed-unexpectedly
```

apt install python3-pip
pip3 --version
pip3 install pyppeteer
python3 picture.pl   # download chrome

# fix browser issue
ldd ~/.local/share/pyppeteer/local-chromium/588429/chrome-linux/chrome
ldd ~/.local/share/pyppeteer/local-chromium/588429/chrome-linux/chrome | grep 'not found'

wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub | sudo apt-key add -
echo 'deb [arch=amd64] http://dl.google.com/linux/chrome/deb/ stable main' | sudo tee /etc/apt/sources.list.d/google-chrome.list
sudo apt update
sudo apt install google-chrome-stable
apt install libxss1
sudo apt install fonts-wqy-zenhei

python3 picture.py   # should work

```

## Face Regnition
pip install opencv-python
pip show opencv-python

https://github.com/opencv/opencv/blob/master/data/haarcascades/haarcascade_frontalface_default.xml

