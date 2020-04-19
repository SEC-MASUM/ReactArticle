## What is Webpack

যত দিন যাচ্ছে তত জাভাস্ক্রিপ্ট উন্নত হচ্ছে এবং জাভাস্ক্রিপ্টকে ঘিরে তৈরি হচ্ছে নানা রকম সব টুলস আমাদের কাজ গুলোকে সহজ করার জন্য। Webpack এমনই একটা টুলস।

Webpack এর মূল দায়িত্ব হচ্ছে কোড গুলোকে বান্ডেলিং করে ফেলা। আমরা যখন একটা প্রজেক্ট করি তখন সেখানে অনেক ফাইল হয়। অর্থাৎ আমরা আমাদের কোড গুলোকে ছোট ছোট ফাইলে ডিস্ট্রিবিউট করে রাখি যেন কোড গুলো ম্যানেজ করতে সহজ হয়। কিন্তু যদি এভাবেই অনেক গুলো ফাইলে কোড রেখে আমরা ওয়েব সাইটকে পাবলিশ করে দেই তাহলে আমাদের ওয়েবসাইট বা ওয়েব অ্যাপ্লিকেশনটার পার্ফরমেন্স ভাল হবে না। কারণ প্রতিটা ছোট ছোট ফাইলের জন্য এর নেটওয়ার্ক কলের প্রয়োজন পরবে। তাই অ্যাপ্লিকেশনটা পাবলিশ করার আগেই আমাদের উচিত হবে সব কোড গুলোকে মিনিফাই করে, এক জায়গাতে বান্ডেল করে তারপরে পাবলিশ করা।

এই কাজটা যদি আমরা ম্যানুয়ালি করতে চাই, তাহলে আমাদের অনেক সময় লাগবে এবং কাজটাও ভাল ভাবে হবে না। এই জন্য আমাদের হয়ে এই কাজটা সুন্দর ভাবে করে দিচ্ছে Webpack।

Webpack ব্যবহার করে আমরা মূলত অনেক গুলো কাজ করে থাকি -

- কোড বান্ডেলিং
- মিনিফাইং
- সোর্স ম্যাপ তৈরি
- ইমেজ এবং কোড অপটিমাইজেশন
- সিএসএস মডিউল
- ডেভেলপমেন্ট সার্ভার
- আরও অনেক কিছু
Webpack মূলত একটা নোডজেএস এর প্যাকেজ যা রান করে নোডজেএস প্লাটফর্মে। আমাদেরকে একটা কনফিগারেশন ফাইল তৈরি করতে হয় প্রজেক্ট অনুযায়ী। তারপরে বিউল্ড কমান্ড দিয়ে আমাদের কনফিগারেশন অনুযায়ী প্রজেক্টটাকে বিউল্ড করতে পারি।

Webpack সম্পর্কে বিস্তারিত জানতে এর অফিশিয়াল ডকুমেন্টেশন ফলো করুন। আর যদি Webpack শিখতে চান তাহলে এই ভিডিওটা দেখে আসতে পারেন। Link: https://youtu.be/PhuwlYrd-XU