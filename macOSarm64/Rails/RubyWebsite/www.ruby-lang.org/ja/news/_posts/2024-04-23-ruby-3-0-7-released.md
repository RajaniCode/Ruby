---
layout: news_post
title: "Ruby 3.0.7 リリース"
author: "hsbt"
translator: "HiroyasuTawwara"
date: 2024-04-23 10:00:00 +0000
lang: ja
---

Ruby 3.0.7 がリリースされました。

このリリースでは以下の脆弱性修正が含まれています。
詳しくは以下の記事を参照してください。

* [CVE-2024-27282: 正規表現検索における任意のメモリアドレス読み取りの脆弱性]({%link ja/news/_posts/2024-04-23-arbitrary-memory-address-read-regexp-cve-2024-27282.md %})
* [CVE-2024-27281: RDoc 内の .rdoc_options におけるRCE 脆弱性]({%link ja/news/_posts/2024-03-21-rce-rdoc-cve-2024-27281.md %})
* [CVE-2024-27280: StringIOにおけるバッファーオーバーリード脆弱性]({%link ja/news/_posts/2024-03-21-buffer-overread-cve-2024-27280.md %})

詳しくは [GitHub releases](https://github.com/ruby/ruby/releases/tag/v3_0_7) を参照してください。

このリリースをもって、Ruby 3.0 系列は EOL となります。即ち、Ruby 3.0.7 が Ruby 3.0 系列の最後のリリースとなる予定です。
これ以降、仮に新たな脆弱性が発見されても、Ruby 3.0.8 などはリリースされません (ただし、深刻なリグレッションが発見された場合にはリリースする可能性があります)。すべての Ruby3.0 ユーザーの皆様は、速やかに 3.3、3.2、3.1 への移行を開始することをお勧めします。

## ダウンロード

{% assign release = site.data.releases | where: "version", "3.0.7" | first %}

* <{{ release.url.gz }}>

      SIZE: {{ release.size.gz }}
      SHA1: {{ release.sha1.gz }}
      SHA256: {{ release.sha256.gz }}
      SHA512: {{ release.sha512.gz }}

* <{{ release.url.xz }}>

      SIZE: {{ release.size.xz }}
      SHA1: {{ release.sha1.xz }}
      SHA256: {{ release.sha256.xz }}
      SHA512: {{ release.sha512.xz }}

* <{{ release.url.zip }}>

      SIZE: {{ release.size.zip }}
      SHA1: {{ release.sha1.zip }}
      SHA256: {{ release.sha256.zip }}
      SHA512: {{ release.sha512.zip }}

## リリースコメント

Ruby 開発者の皆様、バグや脆弱性を報告してくれたユーザーの皆様のご協力により本リリースは行われています。
皆様のご協力に感謝します。
