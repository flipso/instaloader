Hey Folks,

this is a fork of https://github.com/instaloader/instaloader

I would ask to become contributer but im not familiar with these GIT stuff. I come from the Subversion world and im learning GIT rn.

---

The code is a good starting point for my data mining plans. However, testing has already shown that some serious beginner mistakes have been made.

On the one hand the encoding is flawed(How is these possible 19k Downloads per month and nobody see that?!) On the other hand I discovered code redundancy. The method json.dumps is called several times. It also instantiates filewriters

I have already fixed the encoding problems and will now check how to dump the comments via structures.py to reduce redundancy

Afterwards I will try to rework the code so that not every post gets its own JSON. But since the code is badly designed for this USE-Case, I will have to tinker with it due to lack of time

The easiest thing to do after all JSONs have been written is to parse those JSONS to exactly one file. But I would only do that as ultima ratio

Cheers,
Flipso

Roadmap
---
- Fixing encoding Issues ✔
- Adding new options for followers/followee ❌
- Dump comments with structures.py ❌
- Parsing JSON files into one file ❌


Disclaimer
----------

.. disclaimer-start

Instaloader and this fork is in no way affiliated with, authorized, maintained or endorsed by Instagram or any of its affiliates or
subsidiaries. This is an independent and unofficial project. Use at your own risk.

Instaloader is licensed under an MIT license. Refer to ``LICENSE`` file for more information.

.. disclaimer-end


