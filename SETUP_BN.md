# Upgrade Lab Gaming GitHub Pages

এই প্যাকেজে তিনটি public তথ্যের পেজ এবং তাদের stylesheet আছে। অ্যাপের ব্র্যান্ড হিসেবে Upgrade Lab Gaming এবং GitHub account হিসেবে mahabub-automation ব্যবহার করা হয়েছে। Support ও privacy request-এর যোগাযোগপথ হিসেবে নতুন repository-র GitHub Issues লিংক রাখা হয়েছে।

## ১. Repository তৈরি

GitHub-এ নতুন repository তৈরি করুন।

- Owner হিসেবে mahabub-automation নির্বাচন করুন।
- Repository name দিন upgrade-lab-gaming।
- Visibility হিসেবে Public নির্বাচন করুন।
- Add README চালু করুন, যাতে main branch তৈরি থাকে।
- Create repository চাপুন।

Public repository-তে এই প্যাকেজের static ওয়েবসাইট ফাইলগুলো প্রকাশ করুন।

## ২. ফাইল যোগ

ZIP extract করে নিচের ফাইলগুলো main branch-এর root-এ যোগ করুন।

- index.html
- privacy.html
- terms.html
- styles.css
- .nojekyll

নতুন repository তৈরি হওয়ার পরে ChatGPT-এর সংযুক্ত GitHub দিয়ে এই ফাইলগুলো যোগ করা যাবে। ফাইলের ওয়েবসাইট লেখা প্রকাশের আগে আপনার প্রকৃত ডেটা ব্যবহারের সঙ্গে মিলিয়ে পড়ুন।

## ৩. GitHub Pages চালু

Repository → Settings → Pages খুলুন।

- Build and deployment-এর Source হিসেবে Deploy from a branch নির্বাচন করুন।
- Branch হিসেবে main নির্বাচন করুন।
- Folder হিসেবে / (root) নির্বাচন করুন।
- Save চাপুন।

সফল deployment-এর পরে GitHub Pages settings-এ দেখানো live URL খুলুন। এই account ও repository নাম ব্যবহার করলে প্রত্যাশিত ঠিকানাগুলো নিচে দেওয়া আছে। সাইট live হওয়ার পরে প্রতিটি পেজের HTTP response এবং লেখা যাচাই করুন।

| ব্যবহার | প্রত্যাশিত URL |
| --- | --- |
| Homepage | https://mahabub-automation.github.io/upgrade-lab-gaming/ |
| Privacy policy | https://mahabub-automation.github.io/upgrade-lab-gaming/privacy.html |
| Terms | https://mahabub-automation.github.io/upgrade-lab-gaming/terms.html |

## ৪. Google OAuth-এর পরবর্তী ধাপ

ওপরের ঠিকানাগুলো deployment-এর পরিকল্পনা। GitHub repository তৈরি বা Pages চালু করার আগে এগুলো ব্যবহারযোগ্য হওয়ার নিশ্চয়তা নেই।

Google Cloud-এর Branding পেজে live পেজগুলোর URL দেওয়া যায়। Authorised domain হিসেবে scheme বা repository path ছাড়া হোস্টনেম ব্যবহৃত হয়। Google আপনার domain গ্রহণ করছে কি না এবং verification চাইছে কি না সেই স্ক্রিন থেকে যাচাই করুন।

Google-এর domain-verification নির্দেশনায় Search Console-এর Domain property এবং DNS TXT verification চাওয়া হয়েছে। সাধারণ github.io subdomain-এর DNS ব্যবহারকারী পরিচালনা করেন না। তাই GitHub Pages-এ পেজ চালু হওয়া এবং Google OAuth-এর domain গ্রহণ করা আলাদা যাচাই। নিজস্ব domain-এর DNS access প্রয়োজন হলে সেই domain GitHub Pages-এ যুক্ত করে একই ফাইল প্রকাশ করা যায়।

Application home page, privacy ও terms একই সাইটের মধ্যে রাখুন। নতুন domain ব্যবহার করলে GitHub Pages custom-domain setup এবং Google-এর ownership verification শেষ করুন।

## পেজের তথ্য

পেজগুলো বর্তমান uploader-এর কাজের ভিত্তিতে লেখা হয়েছে। Google OAuth-এর youtube.upload এবং youtube.readonly permissions, স্থানীয় credentials ও upload receipts, এবং Telegram notifications-এর তথ্য উল্লেখ আছে। ব্যক্তিগত contact email-এর পরিবর্তে project Issues ব্যবহার করা হয়েছে।

ডেটা ব্যবহার বা retention বদলালে privacy policy-ও হালনাগাদ করুন। GitHub hosting ও Google OAuth approval বাস্তব external setup সম্পন্ন হলে আলাদাভাবে যাচাই করতে হবে।

## প্রাসঙ্গিক নথি

- https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages
- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
- https://support.google.com/cloud/answer/15549049?hl=en
- https://support.google.com/cloud/answer/13804266?hl=en
- https://developers.google.com/identity/protocols/oauth2/production-readiness/brand-verification
