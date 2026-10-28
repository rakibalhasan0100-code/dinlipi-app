দিনলিপি — Android-এ ইনস্টল করার জন্য প্রস্তুত PWA প্যাকেজ

ফাইল:
- index.html — সম্পূর্ণ অ্যাপ ও ইনস্টল বোতাম
- manifest.json — PWA metadata ও app icons
- sw.js — service worker / cache
- icons/icon-192.png এবং icons/icon-512.png — ইনস্টল আইকন

লোকালি পরীক্ষা:
1. ZIP Extract করুন।
2. index.html ডাবল-ক্লিক করে মূল ফিচারগুলো পরীক্ষা করুন। সরাসরি file:// থেকে install prompt/service worker কাজ করবে না।

সবার জন্য অনলাইনে প্রকাশ (ফ্রি GitHub Pages):
1. GitHub অ্যাকাউন্টে সাইন ইন করুন।
2. New repository তৈরি করুন; নাম দিন dinlipi-app; Public নির্বাচন করুন।
3. এই ZIP Extract করে সব ফাইল ও icons ফোল্ডার repository-র root-এ আপলোড করুন।
4. Commit changes করুন।
5. Repository Settings → Pages খুলুন।
6. Build and deployment-এ Deploy from a branch নির্বাচন করুন; Branch: main এবং folder: /(root) নির্বাচন করে Save করুন।
7. GitHub প্রকাশের URL দেখাবে; প্রকাশ হতে কয়েক মিনিট লাগতে পারে।
8. প্রকাশিত HTTPS URL Android Chrome-এ খুলুন → Install app অথবা ⋮ → Add to Home screen নির্বাচন করুন। উপযুক্ত ব্রাউজারে হেডারের “ইনস্টল” বোতামও দেখা যাবে।

গুরুত্বপূর্ণ:
- GitHub Pages সাধারণত public repository থেকে ফ্রি-তে static site হোস্ট করে।
- এই ধাপগুলো নিজে GitHub-এ লগইন করে করতে হবে; এই চ্যাট থেকে তোমার অ্যাকাউন্টে অনুমতি ছাড়া প্রকাশ করা হয়নি।
- অ্যাপের তথ্য localStorage-এ, তাই প্রতিটি ব্যবহারকারীর তথ্য তার নিজস্ব ব্রাউজার/ডিভাইসে থাকবে। এখনো লগইন, ক্লাউড সিঙ্ক বা পুশ নোটিফিকেশন নেই।
- PWA ইনস্টলযোগ্য হতে HTTPS এবং সঠিক manifest/icon দরকার; browser অনুযায়ী install UI ভিন্ন হতে পারে।
