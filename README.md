# timer
The timer.js is a simple then useful JavaScript Timer...

Usage:
step1: 引入 js 文件
<script type="text/javascript" src="./path/to/timer.js"></script>

step2: 使用 Timer 倒计时功能
<pre>
<script type="text/javascript">

  // 定义一个变量，表示 30 秒的倒计时起始时间
  var timeout = 30;

  Timer.stop().run(timeout, function(){
    // 此函数封装倒计时期间要执行的代码, 如：
    $('#test span').fadeOut('normal').html(Timer.tm); // 事先加载 jQuery 库, 获取 DOM 的 id 为 test 的节点，显示它并向其中实时写入倒计时的剩余时间
  }, function() {
    // 此函数封装倒计时结束时要执行的代码, 如：
    // 倒计时结束，隐藏显示剩余时间的 DOM 节点
    $('#test span').fadeOut('normal');
  });

</script>
</pre>

enjoy it!
