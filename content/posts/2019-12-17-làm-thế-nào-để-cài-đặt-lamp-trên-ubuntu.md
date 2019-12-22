---
template: "post"
title: Làm thế nào để cài đặt LAMP trên Ubuntu
slug: lam-the-nao-de-cai-lamp
draft: false
date: 2019-12-17T02:08:45.664Z
description: Cách để cài đặt LAMP trên ubuntu
category: UBUNTU
tags:
  - LAMP
---
Bộ cài đặt LAMP là 1 bộ cài phần mềm mã nguồn mở, nó giúp bạn có thể tạo websites và ứng dụng web. LAMP là từ viết tắt của 1 bộ bao gồm hệ điều hành Linux, Apache server, hệ quản trị cơ sở dữ liệu MySQL, và ngôn ngữ lập trình PHP.

Để cài đặt LAMP trên máy tính của bạn làm theo các bước sau:

## **Bước 1: cập nhật hệ thống của bạn:**

sudo apt-get update

## **Bước 2: Cài đặt MySQL:**

sudo apt-get install mysql-server mysql-client libmysqlclient-dev

## **Bước 3: Cài đặt Apache server:**

sudo apt-get install apache2 apache2-doc apache-npm-prefork

Apache2-utils libexpat1 ssl-cert

## **Bước 4: Cài đặt PHP (phiên bản php 7,0 hoặc mới hơn của php ):**

sudo apt-get install libapache2-mod-php7.0 php7.0 php7.0-common php7.0-curl php7.0-dev php7.0-gd php-pear php-imagick php7.0-mcrypt php7.0-mysql php7.0-ps php7.0-xsl

## **Bước 5: cài đặt phpmyadmin (cho cơ sở dữ liệu)**

sudo apt-get install phpmyadmin



Source: https://medium.com/better-programming/how-to-install-lamp-stack-on-ubuntu-db77ac018116

Translator by: Đông đẹp trai :V
