##基于html5的播放器
[演示地址](https://fzninja.github.io/#/assembly/fz-video)
####在head标签内引入fz-video.css与iconfont.css
		<link rel="stylesheet" href="./fz-video.css">
		<link rel="stylesheet" href="./font/iconfont.css">
####在body底部引入fz-video.js
		<script src="./fz-video.js"></script>
####随后实例化播放器即可
		<script>
			var FZ_VIDEO = new createVideo(
	 		"testBox",	//容器的id
		 		{
		 			url 		: 'http://171.15.197.89/xdispatch/o8t28neoq.bkt.clouddn.com/test.mp4', 	//视频地址
		 			autoplay	: true			//是否自动播放
		 		}
	 		);
	 	</script>
####参数说明
		createVideo的第一个参数为播放器容器的id,播放器宽高等同于容器的宽高
		url			: 视频的地址
		autoplay	: 视频准备就绪后,是否自动播放,true为自动播放,否则false
####方法说明
		var FZ_VIDEO = new createVideo(参数);	//实例化并创建播放器

		FZ_VIDEO.setUrl("URL");		//切换视频,传入视频地址进行切换
		FZ_VIDEO.overVideo();		//移除播放器,且销毁实例,销毁后可重新进行实例化播放器