



## Downloading Videos from Youtube With Python

I am writing a method which will download videos from youtube..$ab=1;$

> this is a Qoute

```python
from pytube import YouTube
from pprint import pprint

yt = YouTube("https://www.youtube.com/watch?v=3W5ovvdHoEY")
print(yt.get_videos())
print(yt.filename)
yt.set_filename('python download')
print(yt.filter('flv'))
print(yt.filter('mp4')[-1])
print(yt.filter(resolution='720p'))
video = yt.get('mp4', '720p')
print(yt.videos)
video.download('E:/')
```


