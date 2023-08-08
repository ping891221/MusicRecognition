
建議先建虛擬環境

## 要用的套件:

```
sudo apt-get install python-tk
sudo apt install ffmpeg
sudo apt-get install portaudio19-dev python3-pyaudio
```
接下來
```
pip -r requirements.txt
```

## clone他
```
git clone https://github.com/ping891221/MusicRecognition.git
```

## Generate MP3 files fingerprints
/mp3裡面有放預計要使用的音檔
```
python collect-fingerprints-of-songs.py
```
查看資料庫
```
python get-database-stat.py
```
## Recognizing audio from microphone
可以自己設定秒數，如果不輸入秒數會不斷監聽直到手動停止
```
python recognize-from-microphone.py -s 5
```
## 
原本的教程(https://ourcodeworld.com/articles/read/973/creating-your-own-shazam-identify-songs-with-python-through-audio-fingerprinting-in-ubuntu-18-04)
