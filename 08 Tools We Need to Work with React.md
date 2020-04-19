## Tools We Need to Work with React
React খুবই ছোট একটা লাইব্রেরী। শুধুমাত্র ইন্টারেক্টিভ UI ডিজাইন করার জন্য এই লাইব্রেরীটা তৈরি করা হয়েছে। তাই সম্পূর্ণ ওয়েব অ্যাপ্লিকেশন বানানোর জন্য যা যা সুযোগ সুবিধা দরকার তা বিউল্ট ইন ভাবে React এ নেই। React খুব ছোট্ট একটা দায়িত্ব পালন করে, আর এই ছোট্ট দায়িত্বটা সে খুব যত্নের সাথে ভাল ভাবে পালন করে, আর তাই তো React এত জনপ্রিয়। তবে ওয়েব অ্যাপ্লিকেশন বানানোর জন্য তো আমাদের আরও অনেক ফিচার দরকার, সেই গুলোর সল্যুশন কিভাবে করব?

এই লেসনে আমরা সেই বিষয়েই আলোচনা করতে যাচ্ছি। React একটা লাইব্রেরী, এর সাথে আমাদের পছন্দ মত টুলস ব্যবহার করে আমরা একটা কাস্টম ফ্রেমওয়ার্ক বানিয়ে ফেলতে পারি। যদি ও এই গুলো আপনার এখনই দরকার পরবে না, যখন আপনি পুরোপুরি ভাবে React শিখে ফেলবেন তখনই শুধু এই গুলো দরকার পরবে। কিন্তু আপনাদের জ্ঞাতার্তে, যেন আপনাদের React এর সাথের যাত্রাটা পরিকল্পনা করতে সহজ হয় তাই আমি এখনি আপনাদের কে বিষয় গুলো জানিয়ে রাখছি।

আমি এখানে যেই টুলস গুলোর কথা বলবো সেই গুলোই যে আপনাকে ব্যবহার করতে হবে এমনটা না। এই টুলসটা যেই প্রব্লেমটা সলভ করছে সেই একই সলভ করতে পারে এমন যে কোনো টুলস আপনি ব্যবহার করতে পারেন। এখানে আমি শুধু মাত্র প্রধান প্রব্লেম গুলোর কথাই উল্লেখ করছি, এছাড়াও আপনি যখন ডেভেলপমেন্ট করবেন তখন আরও অনেক রকম প্রব্লেম এর সম্মুখীন হতে পারেন। সেই সময় আপনার প্রয়োজন অনুযায়ী সঠিক টুলটা আপনাকেই খুঁজে নিতে হবে। তবে ভয় পাওয়ার কিছু নেই, সম্ভাব্য সকল প্রব্লেম এর সমাধান আগেই থেকেই হয়ে আছে, আপনাকে শুধু খুঁজে নিতে হবে।

প্রধান প্রব্লেম গুলো যা না হলে ওয়েব অ্যাপ্লিকেশন হবে না, কিন্তু সে গুলো React এর সাথে বিউল্ট ইন ভাবে নেই -

- AJAX: React অ্যাপ্লিকেশনে সার্ভার থেকে ডাটা নিয়ে এসে ব্রাউজারে দেখানো বা ইউজার এর তৈরি করা ডাটা সার্ভারে পাঠানোর জন্য ব্যবহার করা হয় AJAX. এই জন্য আপনি ব্যবহার করতে পারেন Fetch API অথবা Axios লাইব্রেরী। React এ AJAX এর জন্য বিউল্ট ইন কোনো সমাধান দেওয়া নেই।
- Routing: যখন আপনি সিঙ্গেল পেজ অ্যাপ্লিকেশন বানাবেন তখন আপনাকে ক্লাইন্ট সাইডে রাউটিং করার প্রয়োজন পরবে। অর্থাৎ বিভিন্ন রাউটের জন্য বিভিন্ন পেজ রেন্ডার করার সিস্টেম দরকার পরবে। React এর জন্য কোনো সমাধান নেই। আপনি থার্ড পার্টি টুলস হিসেবে React Router 5 or Reach Router ব্যবহার করতে পারেন।
- Redux: অ্যাপ্লিকেশন যখন বড় হয়ে যায় তখন অ্যাপ্লিকেশনের ডাটা ম্যানেজ করা খুব কষ্টকর ব্যাপার হয়ে যায়। React এ বিউল্ট ইন ভাবে যে সমাধান দেওয়া আছে, তা এই প্রব্লেম এর সমাধান করতে পারে না। তাই আমাদের দরকার হয় কোনো একটা স্টেট ম্যানেজমেন্ট টুল। এই কাজের জন্য জনপ্রিয় লাইব্রেরী হচ্ছে Redux। কিন্তু আপনি আপনার পছন্দ মত যে কোনো একটা স্টেট ম্যানেজমেন্ট লাইব্রেরী ব্যবহার করতে পারেন।
- Responsive CSS Frameworks: React আপনার অ্যাপ্লিকেশন কে রেস্পন্সিভ করবে না। এর জন্য আপনার অন্য কোনো একটা টুলস এর সাহায্য নিতে হবে। আপনি Bootstrap এর সাহায্য নিতে পারেন, Bootstrap কে  React এর জন্য আলাদা ভাবে ইমপ্লিমেন্ট করে বানানো হয়েছে ReactStrap। এটা খুবই ভাল একটা লাইব্রারি যদি আপনি আগে থেকেই Bootstrap জেনে থাকেন। কিন্তু আমার সাজেশন হল এর সাথে সাথে Material UI টা শিখবেন। এটা খুবই জনপ্রিয় একটা ফ্রেমওয়ার্ক।

এই গুলোই হল প্রধান প্রব্লেম যে গুলোর সমাধান React আগে থেকে করে দিলে আমাদের জন্য ভাল হত। কিন্তু না করাতে ও খারাপ কিছু হয়নি। আমরা এখন আমাদের পছন্দ মত যে কোনো টুলস ব্যবহার করে কাজ করতে পারছি। এছাড়া আপনার বিভিন্ন সময় বিভিন্ন ইউটিলিটি লাইব্রেরী এর সাহায্য নিতে হতে পারে।