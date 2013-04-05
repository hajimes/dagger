Dagger
======

Android でも動作する高速・軽量な依存性注入 Java ライブラリ [Dagger][1] の非公式な日本語情報を提供するプロジェクトです。

詳細な情報については、 [ユーザーガイド日本語訳][2] を、最新および正確な情報についてはオリジナルのサイトを参照してください。


ダウンロード
--------

アプリケーションのランタイム環境に dagger-${dagger.version}.jar を含める必要があります。
そのほか、コード生成を有効化するために、コンパイル時に
dagger-compiler-${dagger.version}.jar を含めてビルドする必要があります。

Maven プロジェクトで利用する場合、 pom.xml の依存関係を記述する節にランタイムを含め、
さらに <code>dagger-compiler</code> アーティファクトを "optional" もしくは "provided" の依存性として含めるとよいでしょう。
（${dagger.version} を、今ある適当なリリースのバージョン番号に置き換えてください）

```xml
<dependencies>
  <dependency>
    <groupId>com.squareup</groupId>
    <artifactId>dagger</artifactId>
    <version>${dagger.version}</version>
  </dependency>
  <dependency>
    <groupId>com.squareup</groupId>
    <artifactId>dagger-compiler</artifactId>
    <version>${dagger.version}</version>
    <optional>true</optional>
  </dependency>
</dependencies>
```

また、ダウンロード可能な .jar ファイルは、 Maven のセントラルリポジトリにあります。
[Dagger](http://search.maven.org/#search%7Cga%7C1%7Cg%3A%22com.squareup%22%20dagger) と
[JavaWriter](http://search.maven.org/#search%7Cga%7C1%7Ca%3A%22javawriter%22) の両方が必要になります。


ライセンス
-------

    Copyright 2012 Square, Inc.

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.


 [1]: https://github.com/square/dagger
 [2]: http://hajimes.github.com/dagger/
 [2]: http://github.com/square/dagger/downloads

