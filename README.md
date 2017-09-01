# 任务描述
- 参考以下示例代码，补充其中的JavaScript功能，完成一个JavaScript代码的编写
- 本任务完成的功能为：用户可以在输入框中输入任何内容，点击“确认填写”按钮后，用户输入的内容会显示在“您输入的值是”文字的右边
```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>IFE JavaScript Task 01</title>
  </head>
<body>

  <label>请输入北京今天空气质量：<input id="aqi-input" type="text"></label>
  <button id="button">确认填写</button>

  <div>您输入的值是：<span id="aqi-display">尚无录入</span></div>

<script type="text/javascript">


  /*    
  在注释下方写下代码
  给按钮button绑定一个点击事件
  在事件处理函数中
  获取aqi-input输入的值，并显示在aqi-display中
  */

 document.getElementById("button").onclick = function () {
                var info=document.getElementById("aqi-input").value;
                if(info==""){
                    document.getElementById("aqi-display").innerHTML ="尚无录入";
                }else{
                    document.getElementById("aqi-display").innerHTML = info;
                }

               
            }

</script>
</body>
</html>
```
