

### w:1024 h:576  -> w:576 h:1024 변형

-t 옵션 : 5초만 인코딩

```
ffmpeg -i input.mp4 -vf "scale=576:1024,setsar=1" -t 5 -c:v libx264 -preset fast -crf 23 -c:a aac -b:a 128k output.mp4
```

