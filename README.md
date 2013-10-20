Homography2
===========

射影変換  透明化対応

透明画像(ボール)に対応しました。  

技術的には、putImageDataで描画すると透明部分は黒色になってしまいます。  
そこで隠しCanvasを用意し、そこに一旦putImageDataで描画させます。  
その後、隠しCanvasから表示CanvasにdrawImageで描画することで透明部分が反映されるようになります。
