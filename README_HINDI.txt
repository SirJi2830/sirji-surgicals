SIR JI SURGICALS BILLING — मोबाइल होम-स्क्रीन ऐप पैकेज

इस ZIP में index.html (मौजूदा बिलिंग ऐप), manifest.webmanifest, sw.js और icon शामिल हैं।

जरूरी: Android Chrome में "Add to Home screen" / इंस्टॉल विकल्प पाने और ऑफलाइन PWA सुविधाओं के लिए इसे HTTPS वेबसाइट पर होस्ट करना जरूरी है। ZIP को सीधे खोलने से इंस्टॉल होने वाला ऐप नहीं बनेगा।

मोबाइल से इस्तेमाल का सरल तरीका:
1. ZIP को डाउनलोड करके Extract करें।
2. फाइलें किसी HTTPS static hosting पर अपलोड करें (जैसे GitHub Pages; इसके लिए अकाउंट और repository सेटअप चाहिए)।
3. प्रकाशित HTTPS लिंक Android Chrome में खोलें।
4. Chrome के ⋮ मेनू में "Add to Home screen" या "Install app" चुनें।
5. ऐप में बिल बनाने से पहले test bill बनाकर PDF, CSV/JSON backup और data restore की जाँच करें।

डेटा सुरक्षा:
- बिलों का डेटा ब्राउज़र के स्थानीय storage में रह सकता है; ऐप हटाने/ब्राउज़र डेटा साफ करने से डेटा खो सकता है। नियमित JSON backup रखें।
- GSTR-1 JSON को GST Portal की वर्तमान Offline Utility में validate किए बिना upload न करें।
- यह package खुद से प्रकाशित नहीं है और कोई public URL/APK इसमें शामिल नहीं है।


PWA INSTALL FIX: manifest.webmanifest now includes 192x192 and 512x512 PNG icons. Upload/replace all files in GitHub repository root, including icons/icon-192.png, icons/icon-512.png, manifest.webmanifest, sw.js, and index.html. Then wait for Pages deployment and reload the site.
