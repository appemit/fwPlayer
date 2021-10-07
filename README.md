# fwPlayer
支持各种最新浏览器的视频和音频的录制、转码、流式传输。可以支持avi MP4(x264,x265) webm mpeg-1 mpeg-2,pcm adpcm mp3 aac wav ogg flac,gif,srt ass等
	 需要延迟 转码的时间,内容小于1G ,或者分段
## 步骤
###1  在服务器端增加反馈的 headers 
	   Cross-Origin-Embedder-Policy: require-corp 
	   Cross-Origin-Opener-Policy: same-origin 

###2  在服务器端（Nginx、apache配置文件mime.types），增加MIME类型，以便支持Content-Type对应的wasm, 增加设置  	
		  文件扩展名Extensions   内容类型 MIME type
		  wasm   application/wasm
 
###3 引入js，配置userAuth 。
###4 初始化init ,然后获得转码AppFW.getData的数据，直接播放


 
  
