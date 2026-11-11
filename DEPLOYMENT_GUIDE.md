# দুর্গাপুর এন্টারপ্রাইজ (Durgapur Enterprise POS) - ওয়েব ডিপ্লয়মেন্ট ও হোস্টিং গাইড

এই সফটওয়্যারটি সম্পূর্ণ স্বয়ংসম্পূর্ণ একটি POS (Point of Sale), ইনভেন্টরি, হিসাবরক্ষণ ও ক্লাউড সিঙ্ক সমৃদ্ধ ওয়েব অ্যাপ্লিকেশন। আপনি খুব সহজেই এটিকে যেকোনো ক্লাউড হোস্টিং, নিজস্ব সার্ভার বা cPanel-এ ডিপ্লয় করতে পারবেন।

---

## 🌟 ১. বর্তমান লাইভ ক্লাউড লিংক (Already Live & Running)
গুগল ক্লাউড রান সার্ভারে আপনার এই অ্যাপ্লিকেশনটি সার্বক্ষণিক সক্রিয় রয়েছে:
🔗 **লাইভ অ্যাপ লিংক:** [https://ais-pre-4bzf7nirucnk2rcfakbafb-762233176609.asia-northeast1.run.app](https://ais-pre-4bzf7nirucnk2rcfakbafb-762233176609.asia-northeast1.run.app)

> এই লিংকে যেকোনো কম্পিউটার, ল্যাপটপ, অ্যান্ড্রয়েড বা আইফোন থেকে সরাসরি লগইন করে ব্যবহার করতে পারবেন। যেকোনো ডিভাইস থেকে তথ্য পরিবর্তন করলে সকল ডিভাইসে তাৎক্ষণিক আপডেট হবে।

---

## 🚀 ২. Vercel বা Netlify-তে ডিপ্লয় করার নিয়ম (১ ক্লিকে সম্পূর্ণ ফ্রি)

### পদ্ধতি ক: Netlify Drop (সবচেয়ে সহজ - কোনো কোডিং লাগবে না)
1. অ্যাপের ভেতর থেকে **হোস্টিং রেডি বিল্ড ফাইল (`durgapur-enterprise-web-dist.zip`)** ডাউনলোড করুন অথবা প্রোজেক্টে `npm run build` রান করে `dist` ফোল্ডারটি নিন।
2. [app.netlify.com/drop](https://app.netlify.com/drop) ওপেন করুন।
3. আপনার আনজিপ করা `dist` ফোল্ডারটি টেনে এনে (Drag & Drop) সেখানে ছেড়ে দিন।
4. মাত্র ১০ সেকেন্ডে আপনার নিজস্ব লাইভ ওয়েবসাইট লিংক তৈরি হয়ে যাবে!

### পদ্ধতি খ: GitHub + Vercel / Netlify
1. আপনার প্রজেক্ট কোড GitHub-এ আপলোড করুন।
2. [vercel.com](https://vercel.com) অথবা [netlify.com](https://netlify.com)-এ লগইন করে **Add New Project** দিন।
3. সেটিংস দিন:
   - **Framework Preset:** `Vite`
   - **Build Command:** `npm run build`
   - **Output Directory:** `dist`
4. **Deploy** বাটনে ক্লিক করুন। ২ মিনিটের মধ্যে অ্যাপ বিশ্বব্যাপী লাইভ হয়ে যাবে।

---

## 🌐 ৩. cPanel বা নিজস্ব ডোমেইন হোস্টিংয়ে ডিপ্লয় (Apache / Nginx / Shared Hosting)

যদি আপনার নিজস্ব ডোমেইন (যেমন: `www.durgapurenterprise.com`) এবং cPanel হোস্টিং থাকে:
1. অ্যাপের ভেতর থেকে **`durgapur-enterprise-web-dist.zip`** ফাইলটি ডাউনলোড করুন (অথবা `npm run build` চালিয়ে `dist` ফোল্ডারের ফাইলগুলো জিপ করুন)।
2. আপনার cPanel-এ লগইন করে **File Manager** খুলুন।
3. `public_html` ফোল্ডারে প্রবেশ করুন (অথবা কোনো সাব-ডোমেইনের ফোল্ডারে)।
4. জিপ ফাইলটি Upload করে **Extract** করুন।
5. ব্যস! আপনার নিজস্ব ডোমেইন ব্রাউজ করলেই পুরো POS সফটওয়্যারটি চালু হয়ে যাবে।

---

## 🔥 ৪. Firebase Hosting-এ ডিপ্লয় করার নিয়ম

আপনার ফায়ারবেস প্রজেক্টের আইডি: `gen-lang-client-0610787803`

টার্মিনালে নিচের কমান্ডগুলো চালান:
```bash
# ১. ফায়ারবেস টুলস ইনস্টল করুন
npm install -g firebase-tools

# ২. লগইন করুন
firebase login

# ৩. প্রোজেক্ট বিল্ড করুন
npm run build

# ৪. ফায়ারবেস ইনিশিয়ালাইজ করুন
firebase init hosting
# - Public directory: dist
# - Configure as single-page app: Yes
# - Overwrite index.html: No

# ৫. ডিপ্লয় করুন
firebase deploy --only hosting
```

---

## 📱 ৫. PWA হিসেবে মোবাইল ও পিসিতে ইনস্টল
- **Android:** Chrome ব্রাউজারে লিংক ওপেন করে উপরের ডানদিকের (⋮) চেপে **"Install App"** বা **"Add to Home screen"** দিন।
- **Windows / Mac:** Chrome বা Edge ব্রাউজারে লিংক ওপেন করে অ্যাড্রেস বারের ডানপাশে **Install (⊕)** আইকনে ক্লিক করুন।
- এটি ফুলস্ক্রিন সফটওয়্যার হিসেবে ইনস্টল হবে এবং কোনো ব্রাউজার ফ্রেম ছাড়াই নিজস্ব উইন্ডোতে চলবে।
