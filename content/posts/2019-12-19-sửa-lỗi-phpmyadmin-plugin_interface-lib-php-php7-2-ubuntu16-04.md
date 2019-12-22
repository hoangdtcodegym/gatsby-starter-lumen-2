---
template: post
title: 'Sửa lỗi Phpmyadmin [plugin_interface.lib.php] + php7.2+ ubuntu16.04'
slug: fix_bug_phpmyadmin
draft: false
date: 2019-12-19T00:56:03.975Z
description: hướng dẫn sửa lỗi phpmyadmin
category: fix_bug
tags:
  - fix_phpmyadmin
---
_**Warning in ./libraries/plugin_interface.lib.php#532**_

_**count(): Parameter must be an array or an object that implements Countable**_

![](/media/1_sxvfd0kmayr3fbpc-ow5eq.png "lỗi trông như này: ")

nguồn thư viện của phpmyadmin tính sai 1 vài tham số. Nó nằm ở dòng 532, mã này nằm ở đường dẫn: 

**_$ /usr/share/phpmyadmin/libraries/plugin_interface.lib.php_**

![](/media/1_xtr1npkmfpbhah571d3yww.png)

**_if ($options != null && count($options) > 0) {_**

tôi nghĩ trong phiên bản php mới, nó không thể sử dụng count() hoặc sizeof() với kiểu dữ liệu không phải mảng. Truyền tham số array vào để có thể sửa. Sửa xong dạng như này: 

![](/media/1_tcu-qbqz_s3vr5oc763coq.png)

**_if ($options != null && count((array)$options) > 0) {_**

Mong rằng mẹo nhỏ này có thể giúp bạn sửa lỗi.



translator: Đông đẹp trai
