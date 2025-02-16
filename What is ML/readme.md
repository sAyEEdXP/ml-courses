মেশিন লার্নিং এ অভ্যস্ত না এমন অনেকের চোখে মেশিন লার্নিং এর নাম শুনলে প্রথমেই যেই চিত্র ভেসে আসে তা হচ্ছে রোবট বা টার্মিনেটর। রোবটিক্স এ মেশিন লার্নিং এর ভুমিকা আছে কিন্তু মেশিন লার্নিং শুধু মাত্র রোবোটিক্সেই সীমাবদ্ধ নয় বরং আরো অনেক কাজেই মেশিন লার্নিং ব্যবহার করা হয় ।    
জিমেইলের স্পাম ফিল্টার সিস্টেম , ফেক নিউজ ডিটেকশন সিস্টেম এমন অসংখ্য কাজে মেশিন লার্নিং এর ব্যবহার আছে । এই অধ্যায়ে আমরা মেশিন লার্নিং কি , মেশিন লার্নিং কিভাবে কাজ করে , মেশিন লার্নিং এর বিভিন্ন ধরন সম্পর্কে জানব ।   


## মেশিন লার্নিং কি ?
খুব সহজ করে যদি বলি, মেশিন লার্নিং হচ্ছে এক ধরনের কম্পিউটার প্রোগ্রামিং যা ডাটা থেখে মেশিন কোন কিছু শিখে বা মানুষকে সিদ্ধান্ত নিতে সহায়তা করে । 
   
উপরের উদাহরন থেকে যদি আমরা একটা প্রোগ্রাম তৈরী করি যা ইমেইলকে দুইভাগে ভাগ করবে , **গুরুত্বপুর্ন ইমেইল** বা **স্পাম**   
মেশিন লার্নিং এর ভাষায় ডাটাকে বলা হয় **Training Sets** বা **Example**

## কেন মেশিন লার্নিং ?

ধরুন, উপরের উদাহরনটাই আমরা মেশিন লার্নিং ছাড়া ট্রেডিশনাল প্রোগ্রামিং এর মাধ্যমে করব । তাহলে স্টেপ গুলা কি হতে পারে ?  
1. প্রথমেই আপনাকে **Spam** ইমেইল দেখতে কেমন সেটা নিয়ে স্টাডি করতে হবে । আপনি এখান থেকে নির্দিষ্ট কিছু ওয়ার্ড বা Phrase কে নির্বাচন করতে পারেন । উদাহরন হিসাবে, *Debit Card* , *free* এই ধরনের কিছু শব্দ । আপনি আরো এডভান্স কিছু করতে চাইলে যা করতে পারেন সেন্ডার নেমের প্যাটার্ন এনালাইসিস করতে পারেন , ইমেইল বডি এনালাইসিস করতে পারেন । 

2. এইবার আপনার দেখা প্যাটার্ন অনুসারে আপনি একটা প্রোগ্রাম লিখবেন । সেটা যে কোন  ল্যাংগুয়েজে যেকোনভাবেই হতে পারে। প্রোগ্রামের মুল এলগোরিদম হবে যদি এই শব্দ গুলা বা আপনার প্যাটার্ন নির্দিষ্ট কোন ইমেইলে থাকে তাহলে সেটাকে **Spam** হিসাবে স্পাম ফোল্ডারে পাঠিয়ে দিবে । 

3. সবশেষে, আপনি প্রোগ্রামটি টেস্ট করবেন , যতক্ষন পর্যন্ত ভাল ফলাফল আসতেছে না ততক্ষন পর্যন্ত উপরের এক বা দুই নং প্রসেস আপডেট করবেন । 


![alt text](https://github.com/aouwalitshikkha/ml-courses/blob/main/What%20is%20ML/images/traditional-program.jpg 'মেশিন লার্নিং প্রোগ্রামিং এলগোরিদম')

প্রতিনিয়ত Spam Email এর প্যাটার্ন চেঞ্জ হবে , আপনাকে প্রতিবার সব কিছু আপডেট করতে হবে আর সেটা অনেক সময় স্বাপেক্ষ ও কষ্ট সাধ্য বিষয় । কারন অনেক ধরনের প্যাটার্ন আপনাকে এখানে মেইনটেইন করতে হবে ।  এখানে স্পামাররা প্রতিনিয়ত ইমেইল টেমপ্লেট ও স্টাইল চেঞ্জ করবে । আগে  For you লিখলে দেখা যাবে এখন 4U লিখতেছে । এইভাবে করে প্রতিনিয়ত আপনাকে প্রোগ্রাম আপডেট করতে হবে । 



![alt text](https://github.com/aouwalitshikkha/ml-courses/blob/main/What%20is%20ML/images/ml-program.jpg 'ট্রেডিশনাল প্রোগ্রামিং এর ধাপ')

কিন্তু একই প্রোগ্রাম ই যদি আপনি মেশিন লার্নিং দিয়ে করেন তাহলে মেইনটেইন করা সহজ হবে ।  মেশিন লার্নিং অটোমেটিক্যালি এই পরিবর্তন গুলা ধরতে পারবে আর আপনাকে না বলেই সেটা স্পাম হিসাবে স্পাম ফোল্ডারে জমা করবে আর প্রতিনিয়ত নিজেকে আপডেট করবে।   
এই ধরনের জটিল সমস্যা গুলা আমরা মেশিন লার্নিং এর সাহায্যে খুব সহজেই সল্ভ করতে পারি  যা নন-মেশিন লার্নিং প্রোগ্রামের মাধ্যমে সমাধান করা কষ্ট কর । উদাহরন হিসাবে Speech to Text এর ক্ষেত্রে আপনি যখন বলবেন One, Two মেশিন লার্নিং এই শব্দগুলা আলাদাভাবে আইডেন্টিফাই করতে পারবে ।   

আর এই আইডেন্টিফিকেশনের জন্য আপনাকে একটি এলগোরিদম বা সিস্টেম তৈরী করতে হবে । 

## কখন মেশিন লার্নিং ?

এই প্রশ্নের উত্তর আসলে সহজে দেওয়া সম্ভব না । তবে আমার ব্যক্তিগত মতামত হচ্ছে 

1. যখন অনেক ধরনের লিস্ট বা রুলসের বা প্যাটার্ন থাকবে , যা ট্রেডিশনাল প্রোগ্রামিং এ মেইনটেইন করা ঝামেলার হবে, তখন মেশিন লার্নিং আপনার কাজের গতি ও প্রোগ্রামকে অনেক সহজ করে দিতে পারে । 

2. অনেক জটিল সমস্যা যা ট্রেডিশনাল প্রোগ্রামিং এর মাধ্যমে সল্ভ করা সম্ভব না । সে ক্ষেত্রে মেশিন লার্নিং ব্যবহার করা যেতে পারে। 

3. Non-Stable Enviroment: যেখানে ডাটা প্রতিনিয়ত পরিবর্তন হয় সেখানে মেশিন লার্নিং নতুন ডাটাকে এডাপ্ট করার জন্য কার্যকরী । 

## মেশিন লার্নিং এর প্রকারভেদ 

মেশিন লার্নিং কে অনেকেই অনেক দৃষ্টি কোন থেকে অনেকভাবে ভাগ করেছেন । মানুষের Supervision এর উপর নির্ভর করে ভাগ করা যায় তিন ভাগে । আবার অনেকেই এইটাকে চারভাগে ভাগ করেছেচন । 

- Supervised learning
- Unsupervised learning
- Semi-supervised learning
- Reinforcement learning






