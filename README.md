# lisu-oss-sources

LISU ImageOrganizer（AKERU LAB）の配布物に含まれるオープンソースのソフトウェアのうち、ライセンスがソースの提供を求めるものの対応ソースを置くリポジトリです。

## GCC 8.3.0（libgcc_s_seh-1.dll・libstdc++-6.dll）

LISU.exe は ExifTool の Windows 版（Oliver Betz のまとめ）を同梱しています。その中の Strawberry Perl に含まれる `libgcc_s_seh-1.dll` と `libstdc++-6.dll` は GCC 8.3.0 のランタイムで、GPLv3 と GCC Runtime Library Exception 3.1 に従います。GPLv3 第 6 条に従い、対応するソースを Release [`gcc-8.3.0`](https://github.com/fujiruki/lisu-oss-sources/releases/tag/gcc-8.3.0) に置いています。

| ファイル | SHA-256 |
|---|---|
| `gcc-8.3.0.tar.xz`（63,694,700 バイト） | `64baadfe6cc0f4947a84cb12d7f0dfaf45bb58b7e92461639596c21e02d97d2c` |
| `gcc-8.3.0.tar.xz.sig` | `4fac1a2da66a743c7dec0d672e8712bb58791c388fc9ca6510588930d934e11c` |

- 出典: https://ftp.gnu.org/gnu/gcc/gcc-8.3.0/gcc-8.3.0.tar.xz （GNU の公式の配布元。2026-10-15 に取得）
- 署名の確認: `https://ftp.gnu.org/gnu/gnu-keyring.gpg` で `gcc-8.3.0.tar.xz.sig` を確かめ、Jakub Jelinek（鍵の指紋 `33C2 35A3 4C46 AA3F FB29 3709 A328 C3A2 C3C4 5C06`）の正しい署名でした（鍵はすでに期限切れですが、署名は期限内の 2019 年に作られた物です）
- Strawberry Perl が GCC に当てたパッチ（ExifTool に同梱の `Licenses_Strawberry_Perl.zip` の `gcc-toolchain/_INFO_` に一覧があります）は公開の置き場所が見つからないため、GPLv3 第 6 条 (b) の書面の申し出で提供します。配布から 3 年間、求めに応じて対応ソースを無償で提供します。連絡先は LISU の利用規約の問い合わせ先です: https://akerulab.com/products/lisu/legal/terms.html

ライセンスの全文: GPLv3 は https://www.gnu.org/licenses/gpl-3.0.html 、GCC Runtime Library Exception 3.1 は https://www.gnu.org/licenses/gcc-exception-3.1.html 。

このリポジトリのファイルは、LISU の配布を終えてから 3 年以上置きます。
