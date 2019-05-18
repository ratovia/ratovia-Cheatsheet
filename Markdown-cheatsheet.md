# 基本
hello

半角スペース２個で  
改行です。


# H１
## シャープ2個で H2
### シャープ3個で H3

# 引用
> 引用は>です
>>入れ子は>>です

# リスト

* リストは＊です。
  * タブで段落落ちします。

1. 数字のリストは1.です。
  2. タブで段落落ちします。

# チェックボックス

- [ ] - [ ] でチェックボックスになります。
- [x] - [x] でチェックがつきます。 

# リンク

## < url >　でリンクになります。
<http://qiita.com>

## [文字] (url)でリンクになります。
[Qiita](http://qiita.com)

# 強調・打ち消し

**アスタリスク二つで囲むと強調します**
~~チルダ二つで囲むと打ち消しします~~

# コード


`アノテーションで囲むとコードになります`
`int i = 10`

```
html:sample
<div class="radioWave">
  <p>アノテーションで囲むとプログラムになります</p>
</div>
```

    class Hoge
        def hoge
            print 'スペース４つでプログラムになります'
            print 'タブ２つでプログラムになります'
        end
    end

# テーブル

| Left align | Right align | Center align |
|:-----------|------------:|:------------:|
| This       |        This |     This     |
| column     |      column |    column    |
| will       |        will |     will     |

        | Left align | Right align | Center align |
        |:-----------|------------:|:------------:|
        | This       |        This |     This     |
        | column     |      column |    column    |
        | will       |        will |     will     |

# 画像埋め込み
![代替テキスト](画像のURL)

タイトル無しの画像を埋め込む

![代替テキスト](画像のURL "画像タイトル")

タイトル有りの画像を埋め込む