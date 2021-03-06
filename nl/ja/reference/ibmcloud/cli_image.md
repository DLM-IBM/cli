---

copyright:

  years: 2018


lastupdated: "2018-11-29"
---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:tip: .tip}

# コンピュート・イメージの作成、編集、および削除

以下のコマンドを使用して、{{site.data.keyword.Bluemix}} コンピュート・イメージを管理します。
{: shortdesc}

<table summary="コマンドの詳細情報を表示するリンクが含まれたアルファベット順の {{site.data.keyword.Bluemix_notm}} インフラストラクチャー・イメージ・コマンド">
 <tbody>
 <tr>
 <td>[ibmcloud sl image delete](/docs/cli/reference/ibmcloud/cli_image.html#sl_image_delete)</td>
 <td>[ibmcloud sl image detail](/docs/cli/reference/ibmcloud/cli_image.html#sl_image_detail)</td>
 <td>[ibmcloud sl image edit](/docs/cli/reference/ibmcloud/cli_image.html#sl_image_edit)</td>
 <td>[ibmcloud sl image list](/docs/cli/reference/ibmcloud/cli_image.html#sl_image_list)</td>
 </tr>
   </tbody>
 </table>

 ## ibmcloud sl image delete
{: #sl_image_delete}

イメージを削除します。
```
ibmcloud sl image delete IDENTIFIER
```
**例**:
```
   ibmcloud sl image delete 12345678
```
このコマンドは、ID `12345678` のイメージを削除します。

## ibmcloud sl image detail
{: #sl_image_detail}

イメージの詳細を取得します。
```
ibmcloud sl image detail IDENTIFIER
```
**例**:
```
 ibmcloud sl image detail 12345678
```
このコマンドは、ID 12345678 のイメージの詳細を取得します。

## ibmcloud sl image edit
{: #sl_image_edit}

イメージの詳細を編集します。
```
ibmcloud sl image edit IDENTIFIER [OPTIONS]
```

<strong>コマンド・オプション</strong>:
<dl>
<dt>--name</dt>
<dd>イメージの名前。</dd>
<dt>--note</dt>
<dd>イメージの追加のメモ。</dd>
<dt>--tag</dt>
<dd>イメージのタグ。</dd>
</dl>

*例**:
```  
ibmcloud sl image edit 12345678 --name ubuntu16 --note testing --tag staging
```
このコマンドは、ID `12345678` のイメージを編集し、名前を「`ubuntu16`」に設定し、メモを「`testing`」に設定し、タグを「`staging`」に設定します。

## ibmcloud sl image list
{: #sl_image_list}

ご使用のアカウントのすべてのイメージをリストします。
```
ibmcloud sl image list [OPTIONS]
```

<strong>コマンド・オプション</strong>:
<dl>
<dt>--name</dt>
<dd>イメージ名を基準にフィルター操作します。</dd>
<dt>--public</dt>
<dd>パブリック・イメージのみを表示します。</dd>
<dt>--private</dt>
<dd>プライベート・イメージのみを表示します。</dd>
</dl>
