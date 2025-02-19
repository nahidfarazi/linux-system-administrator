শেলের প্রম্পট ব্যবহার করে কমান্ড ইস্যু করা হলো লিনাক্সে কাজ করার একটি প্রধান মাধ্যম। শেলের মাধ্যমে বিভিন্ন
কমান্ড ইস্যু করে আপনি সিস্টেমের সাথে যোগাযোগ করতে পারেন। লিনাক্স শেলে কমান্ডগুলো লিখতে হয় নির্দিষ্ট
সিনট্যাক্স অনুসারে।
নিচে কয়েকটি দেওয়া হলো:
১. শেলের প্রম্পট কীভাবে কাজ করে:
শেলের প্রম্পটটি সাধারণত নিচের মতো দেখা যায়:
``
[user@hostname ~]$
``
এখানে:
●user মানে আপনার ব্যবহারকারী নাম।
●hostname হলো আপনার সিস্টেমের নাম।
●~ চিহ্নটি আপনার বর্তমান ডিরেক্টরিকে নির্দেশ করে (এটি আপনার হোম ডিরেক্টরি)।
●$ চিহ্নটি সাধারণ ব্যবহারকারীর জন্য, আর যদি আপনি root ব্যবহারকারী হন, তবে এটি # থাকবে।
২. কিছু মৌলিক কমান্ড:
ls কমান্ড:
ফাইল এবং ডিরেক্টরির লিস্ট দেখতে:
```sh
ls
```
এটি বর্তমান ডিরেক্টরির ফাইল এবং ফোল্ডারগুলির তালিকা দেখায়।
cd কমান্ড:
ডিরেক্টরি পরিবর্তন করতে:
``
cd /path/to/directory
``
যেমন, আপনার হোম ডিরেক্টরিতে যেতে:
```sh
cd ~
```
pwd কমান্ড:
বর্তমান কাজের ডিরেক্টরি (present working directory) দেখতে:
```sh
pwd
```
এটি আপনাকে বর্তমান ডিরেক্টরির পূর্ণপথ দেখাবে।
mkdir কমান্ড:
নতু ন ডিরেক্টরি তৈরি করতে:
``
mkdir directory_name
``
যেমন, একটি নতুন ফোল্ডার তৈরি করতে:
```sh
mkdir myfolder
```
touch কমান্ড:
ফাইল তৈরি করতে:
``
touch file_name
``
যেমন, একটি নতুন ফাইল তৈরি করতে:
```sh
touch myfile.txt
```
৩. রুট ব্যবহারকারী (সুপার ইউজার) হিসেবে কমান্ড চালানো:সাধারণ ব্যবহারকারীর চেয়ে রুট ব্যবহারকারী অধিক ক্ষমতাসম্পন্ন। কোনো রুট কমান্ড চালাতে হলে sudo
ব্যবহার করতে হয়। যেমন:
``
sudo command_name
যেমন, কোনো প্যাকেজ ইনস্টল করতে:

sudo yum install package_name
``
এখানে yum হলো প্যাকেজ ম্যানেজার, যা লিনাক্সে সফটওয়্যার ইনস্টল করতে সাহায্য করে।
৪. ফাইল দেখার জন্য cat, less, more:
ফাইলের ভেতরের বিষয়বস্তু দেখতে পারেন:
``
cat filename
``
অথবা:
``
less filename
``
less কমান্ডটি বড় ফাইলের জন্য সুবিধাজনক, কারণ এটি ফাইল স্ক্রল করে দেখার সুযোগ দেয়।
৫. শেলের সিনট্যাক্স:
প্রত্যেকটি শেল কমান্ড নির্দিষ্ট সিনট্যাক্স অনুসরণ করে। যেমন, অনেক কমান্ডের সাথে ফ্ল্যাগ বা অপশন ব্যবহার করা
হয়। উদাহরণ:
```sh
ls -l
```
এখানে -l হলো একটি ফ্ল্যাগ, যা কমান্ডের আউটপুট পরিবর্তন করে এবং বিস্তারিতভাবে ফাইলের তথ্য দেখায়।এগুলো হলো শেল কমান্ডের বেসিক ধারণা। আপনি লিনাক্স শেল ব্যবহার করে যেকোনো কাজ করতে পারবেন যদি
এই মৌলিক কমান্ডগুলো ভালোভাবে অনুশীলন করেন।
