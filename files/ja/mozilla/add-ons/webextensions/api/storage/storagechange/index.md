---
title: storage.StorageChange
slug: Mozilla/Add-ons/WebExtensions/API/storage/StorageChange
---

{{AddonSidebar}}

`StorageChange` はストレージ領域の変更を表すオブジェクトです。

## 型

`StorageChange` オブジェクトは以下のプロパティを持ちます。

- `oldValue`{{optional_inline}}
  - : アイテムの変更前の値が存在すれば、この中に入ります。データ型は特定されておらず、何らかのデータ型が入ります。
- `newValue`{{optional_inline}}
  - : アイテムの変更後の値があれば、この中に入ります。データ型は特定されておらず、何らかのデータ型が入ります。

## ブラウザーの互換性

{{Compat}}

{{WebExtExamples}}

> [!NOTE]
> この API は Chromium の [`chrome.storage`](https://developer.chrome.com/docs/extensions/reference/api/storage) API に基づいています。また、このドキュメントは [`storage.json`](https://chromium.googlesource.com/chromium/src/+/master/extensions/common/api/storage.json) における Chromium のコードに基づいています。

<!--
// Copyright 2015 The Chromium Authors. All rights reserved.
//
// Redistribution and use in source and binary forms, with or without
// modification, are permitted provided that the following conditions are
// met:
//
//    * Redistributions of source code must retain the above copyright
// notice, this list of conditions and the following disclaimer.
//    * Redistributions in binary form must reproduce the above
// copyright notice, this list of conditions and the following disclaimer
// in the documentation and/or other materials provided with the
// distribution.
//    * Neither the name of Google Inc. nor the names of its
// contributors may be used to endorse or promote products derived from
// this software without specific prior written permission.
//
// THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
// "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
// LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
// A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
// OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
// SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
// LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
// DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
// THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
// (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
// OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-->
