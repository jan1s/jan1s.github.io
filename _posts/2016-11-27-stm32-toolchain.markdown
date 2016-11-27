---
layout: post
title:  "STM32 Toolchain"
date:   2016-11-27 18:44:26 +0100
categories: jekyll update
---

Setting up a STM32 toolchain can be confusing.
Here is how i do it.

# macOS

If you have not installed [Homebrew][brew] yet, you should do that right now.

Install [stlink][stlink]:
{% highlight bash %}
brew install stlink
{% endhighlight %}

Install GNU ARM GCC Toolchain:
{% highlight bash %}
xcode-select --install
brew tap PX4/homebrew-px4
brew update
brew install genromfs
brew install gcc-arm-none-eabi
{% endhighlight %}

Install eclipse:
{% highlight bash %}
brew tap caskroom/cask
brew cask install java
brew cask install eclipse-cpp
{% endhighlight %}

Install the [GNU ARM Eclipse Plugin][plugin].

In Project Properties -> C/C++ Build -> Environment -> Add:

`Name: PATH`
`Value: /usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin`

Setting up a debug configuration [source][debug]:




[brew]: http://brew.sh
[stlink]: https://github.com/texane/stlink
[plugin]: http://gnuarmeclipse.github.io/plugins/install/
[debug]: http://erika.tuxfamily.org/wiki/index.php?title=Tutorial:_STM32_-_Integrated_Debugging_in_Eclipse_using_GNU_toolchain&oldid=5474

