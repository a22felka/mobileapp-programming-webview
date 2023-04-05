
**Jag började med att forka och klona webview appen från github så att jag själv skulle kunna redigera den. Sedan gick jag in i 
strings filen och bytte ut app namnet "WebViewApp" med "MyWebView."
Jag gick in i activity_main.xml, bytte ut textView mot en webView och tog bort dess text.
Gav appen tillstånd att använda internet i AndroidManifest, tog även bort redundant label i activity samt satte android exported 
till true för att fixa varningar.
La till ett id på WebViewen för att sedan skapa ett privat variabel "myWebView" som använder mitt id för att hitta webview elementet, 
jag initierade även myWebView genom att använda "findViewById(R.Id.my_WebView)."
Använde setWebViewClient för att skapa en ny client och satte ihop den med min WebView.
Satte på javascript i MainActivity.java med hjälp av "getSettings().setJavaScriptEnabled(true)."
Skapade en asset i min app som bara innehåller ett directory med en html fil och använde loadUrl() i onOptionsItemSelected för att 
göra så att knappen "External Web Page" tog dig till his.se och "Internal Web Page" tar dig till html filen i assets.**