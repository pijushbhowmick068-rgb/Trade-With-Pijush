TRADE WITH PIJUSH — Version 1.0
================================

এটি একটি প্রথম working prototype (PWA)। Android ফোনের Chrome browser-এ চালানোর জন্য বানানো।

যা কাজ করে:
- Indian F&O / Forex / Crypto segment switch
- Sample watchlist ও illustrative chart
- Demo Entry / Stop Loss / Target 1, 2, 3
- Risk calculator
- Paper trade journal (এই prototype-এ session memory only)
- PWA manifest ও offline cache

গুরুত্বপূর্ণ:
- কোনো live exchange data নেই।
- কোনো AI prediction বা 80% accuracy claim নেই।
- কোনো broker login/API নেই।
- কোনো real order execute হয় না।
- প্রদর্শিত price ও signal সম্পূর্ণ sample/demo।

Android ফোনে চালানোর সহজ উপায়:
1. ZIP extract করে index.html ও বাকি ফাইলগুলো একসঙ্গে রাখুন।
2. PWA install করতে HTTPS hosting দরকার। GitHub Pages / Netlify-তে project folder publish করুন।
3. Android Chrome-এ published HTTPS link খুলুন।
4. Chrome menu (⋮) > Install app অথবা Add to Home screen চাপুন।

শুধু index.html ফাইল local-এ খুললে dashboard দেখা যাবে, কিন্তু PWA install/offline service worker সব browser-এ কাজ নাও করতে পারে।

পরবর্তী ধাপ:
1. Live market data provider নির্বাচন।
2. Secure Python backend ও database।
3. Broker adapters এবং official API credentials।
4. Backtesting + paper forward-testing।
5. Applicable broker/exchange regulatory requirements মেনে সীমিত live automation।

কখনো API secret, password, PIN বা TOTP seed frontend code-এ রাখবেন না।
