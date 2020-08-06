<!DOCTYPE HTML>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <title>e交易平台</title>
    <script type="text/javascript">
        // 获取终端的相关信息
        var Terminal = {
            // 辨别移动终端类型
            platform : function(){
                var u = navigator.userAgent, app = navigator.appVersion;
                return {
                    // android终端或者uc浏览器
                    android: u.indexOf('Android') > -1 || u.indexOf('Linux') > -1,
                    // 是否为iPhone或者QQHD浏览器
                    iPhone: u.indexOf('iPhone') > -1 ,
                    // 是否iPad
                    iPad: u.indexOf('iPad') > -1
                };
            }
        }
 
        // 根据不同的终端，跳转到不同的地址
        var theUrl = 'https://apps.apple.com/cn/app/id1508099701';
        if(Terminal.platform.android){//安卓端
            //document.write('安卓版APP!');
            theUrl = 'http://app.mi.com/details?id=com.ejy365';
            //location.href = theUrl;
        } else {
            if(Terminal.platform.iPhone){//iPhone端
                theUrl = 'https://apps.apple.com/cn/app/id1508099701';
            }
             location.href = theUrl;
        }
        
    </script>
</head>
<body>
    <!--
 
    -->
</body>
</html>
