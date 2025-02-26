---
layout: news_post
title: "Ruby 2.3.4 发布"
author: "nagachika"
translator: "安道"
date: 2017-03-30 00:00:00 +0000
lang: zh_cn
---

Ruby 2.3.4 发布了。

这一版包含自上一版发布以来的 80 个缺陷修正。详情参见[提交日志](https://github.com/ruby/ruby/compare/v2_3_3...v2_3_4)。

这一版修正了 Symbol#hash 的不确定性。这是一个回归问题，存在于 2.3 系列中 2.3.4 之前的版本中。详情参见 [Bug #13376](https://bugs.ruby-lang.org/issues/13376)。

## 已发现的问题

（添加于 2017 年 4 月 11 号）

Ruby 2.3.4 中发现存在 API 不兼容。这是由于意外地删除了一个叫 `rb_thread_fd_close` 的 API。我们会在下一个版本修复这个问题，如果你遇到这个问题并且需要解决方案的话，请应用这个补丁：

* [修复 rb_thread_fd_close 问题的补丁](https://svn.ruby-lang.org/cgi-bin/viewvc.cgi/branches/ruby_2_3/thread.c?r1=58289&r2=58288&pathrev=58289&view=patch)

## 下载

* [https://cache.ruby-lang.org/pub/ruby/2.3/ruby-2.3.4.tar.bz2](https://cache.ruby-lang.org/pub/ruby/2.3/ruby-2.3.4.tar.bz2)

      SIZE:   14434361 bytes
      SHA1:   f5b18e7149ec7620444c91962e695708829d0216
      SHA256: cd9808bb53824d6edb58beaadd3906cb23b987438ce75ab7bb279b2229930e2f
      SHA512: ad1f16142615498232d0de85149585be1d2c5de2bc40ec160d272a09e098ef6f317d8b25026001735261fd1c5bc0d1f8513a8474e89f0d86eed5b2fe7338d64e

* [https://cache.ruby-lang.org/pub/ruby/2.3/ruby-2.3.4.tar.gz](https://cache.ruby-lang.org/pub/ruby/2.3/ruby-2.3.4.tar.gz)

      SIZE:   17820518 bytes
      SHA1:   d064b9c69329ca2eb2956ad57b7192184178e35d
      SHA256: 98e18f17c933318d0e32fed3aea67e304f174d03170a38fd920c4fbe49fec0c3
      SHA512: 23b68ff1f7ab0323876d6135f232f895a5d5009b4128711a685003563828492afb330e589ca614581a49e43027c34e251d96a3fc10330cdfdd11a2537af0233f

* [https://cache.ruby-lang.org/pub/ruby/2.3/ruby-2.3.4.tar.xz](https://cache.ruby-lang.org/pub/ruby/2.3/ruby-2.3.4.tar.xz)

      SIZE:   11450108 bytes
      SHA1:   8ee952fa7c2466d53868143e867dc08a153e20df
      SHA256: 341cd9032e9fd17c452ed8562a8d43f7e45bfe05e411d0d7d627751dd82c578c
      SHA512: 9e3adc2de6703e50e75db37db2981006d4c69759929d61db6a0d63627cfe5977d0ad66d2c69d7161cfc0c0d1c2cb38e5181a06ccd2790df2f72ec25c2ad01e02

* [https://cache.ruby-lang.org/pub/ruby/2.3/ruby-2.3.4.zip](https://cache.ruby-lang.org/pub/ruby/2.3/ruby-2.3.4.zip)

      SIZE:   19869837 bytes
      SHA1:   47a926289e4f007b1a338617f925dd858ea3da97
      SHA256: e70b716982be704375129d4fc0ef305fd8d8151f64e0fcb12de791ab956a526d
      SHA512: 6fab3a737f494d33f91a40881d4ab16a938e98cf0f344fba90104d5cf9e6d02d7c17f64512c2f1ffd67f64ad5dd38477fab0d17614c1ff22627f18232186315a

## 发布记

此次发布得益于诸多提交者、开发者和用户提供的缺陷报告。感谢你们的贡献！
