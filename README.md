
<html>
<head>
   <title>嵐クイズ</title>
   <script type="text/javascript">
    
    function saiten(){
        var point=0;	//　点数
        var max=100;	//　満点
    
        if(document.quiz.a[0].checked){point+=10;}
        if(document.quiz.b[0].checked){point+=10;}
        if(document.quiz.c[2].checked){point+=10;}
        if(document.quiz.d[0].checked){point+=10;}
        if(document.quiz.e[0].checked){point+=10;}
        if(document.quiz.f[2].checked){point+=10;}
        if(document.quiz.g[1].checked){point+=10;}
        if(document.quiz.h[2].checked){point+=10;}
        if(document.quiz.i[0].checked){point+=10;}
        if(document.quiz.j[0].checked){point+=10;}
    
        if(point==max){
            alert(""+max+"点です。\nおめでとうございます。満点です。");
        }
        else{alert(""+point+"点です。\n残念。またチャレンジしてね。");}
        
    
        //　チェックを初期状態に戻します
        //　いらなきゃ削除してもOK
        document.quiz.a[0].checked=true;
        document.quiz.b[0].checked=true;
        document.quiz.c[0].checked=true;
        document.quiz.d[0].checked=true;
        document.quiz.e[0].checked=true;
        document.quiz.f[0].checked=true;
        document.quiz.g[0].checked=true;
        document.quiz.h[0].checked=true;
        document.quiz.i[0].checked=true;
        document.quiz.j[0].checked=true;
    }
    //-->
    </script>
    </head>
    <body>
        <form name="quiz">
            <P>que1　お芝居の勉強や色々なものを体験するために、ニューヨークに行った3人のメンバーはどの組み合わせ？
            <BR><input type=radio name="a" checked>相葉雅紀・大野智・松本潤
            　<input type=radio name="a">大野智・櫻井翔・二宮和也
            　<input type=radio name="a">相葉雅紀、櫻井翔、松本潤
            <P>que2　二宮和也が好きだった外国人野球選手は？
            <BR><input type=radio name="b" checked>オマリー
            　<input type=radio name="b">カブレラ
            　<input type=radio name="b">T.ウッズ
            <P>que3　大野智が櫻井翔に「嵐5人でBBQをしよう」と言った際に、櫻井翔がそれを反対した理由は？
            <BR><input type=radio name="c" checked>好きなもの（それぞれ焼きたい物）がそれぞれ多い
            　<input type=radio name="c">全員揃わない
            　<input type=radio name="c">まとまらない
            <P>que4　櫻井翔が自分の誕生日に思い出すのは誰?
            <BR><input type=radio name="d" checked>多部未華子
            　<input type=radio name="d">関口メンディー
            　<input type=radio name="d">大野智
            <P>que5　大野智が楽屋でよく頼む出前は？
            <BR><input type=radio name="e" checked>そば
            　<input type=radio name="e">中華丼
            　<input type=radio name="e">牛丼
            <P>que6　同じ草野球チームに所属している2人は？
            <BR><input type=radio name="f" checked>相葉雅紀・櫻井翔
            　<input type=radio name="f">相葉雅紀・松本潤
            　<input type=radio name="f">相葉雅紀・二宮和也
            <P>que7　野球選手ローズのファウルボールが肩に当たったことがあるメンバーは？
            <BR><input type=radio name="g" checked>櫻井翔
            　<input type=radio name="g">相葉雅紀
            　<input type=radio name="g">二宮和也
            <P>que8　櫻井翔が気に入っている東京駅の食べ物屋さんは？
            <BR><input type=radio name="h" checked>マフィン
            　<input type=radio name="h">ラーメン
            　<input type=radio name="h">おにぎり
            <P>que9　二宮和也が一日中ゲームをする際、何があれば大丈夫と言った？
            <BR><input type=radio name="i" checked>お茶
            　<input type=radio name="i">水
            　<input type=radio name="i">ガム
            <P>que10　松本潤が一番多くバレンタインチョコをもらった時代は？
            <BR><input type=radio name="j" checked>幼稚園
            　<input type=radio name="j">小学校
            　<input type=radio name="j">中学校
            <P><input type=button value=" 採点 " onClick="saiten()">
            </form>

</body>
</html>
