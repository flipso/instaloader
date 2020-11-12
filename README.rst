Hey Folks,
this is a fork of https://github.com/instaloader/instaloader

Roadmap
----------
- Fixing encoding Issues ✔ 5b3b30d69b1b21563cef9daff1f5f0b7f57d9040
- Adding new options for followers/followee ✔ 44e9c01eb3dc37d031ab000a83d233ef2802721c
   1. First i changed the behavior to only download the followers/followees profile and not download everything recursively because that leads very fast to overheat. In my eyes the old behavior is not good because there is no USE-Case at all
   2. Your now able to download followers by adding @ behind username
   3. Your now able to download followees & followers at once by combining prefix and suffix for example @username@
- Refactor these options to remove the code redundancy ❌ 
--> Asked for help at https://github.com/instaloader/instaloader/issues/866#issue-741050597

- Dump comments via structures.py ✔
- Parsing JSON files into one file ❌
> after a closer look at the code i come to the conclusion that the task is too time consuming or you would have to mess up too much, so i won't develop it. my parser just has to pull the files one by one and then everything is fine

- Implement TOR (For example if Rate Limit > 300 seconds than new TOR identity to avoid longer waiting times)
 > i will develop this functionality at a different time because i have to turn to other components. You are welcome to take over the development. If so please let me know

Disclaimer
----------

.. disclaimer-start

Instaloader and this fork is in no way affiliated with, authorized, maintained or endorsed by Instagram or any of its affiliates or
subsidiaries. This is an independent and unofficial project. Use at your own risk.

Instaloader is licensed under an MIT license. Refer to ``LICENSE`` file for more information.

.. disclaimer-end

