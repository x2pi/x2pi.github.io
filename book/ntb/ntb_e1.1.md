---
layout: post
creationdate:  2018-01-10 00:00:00 +0700
date_create: 2018-01-06
title: Solutions manual for NTB - 1.1 Divisibility and primality
permalink: /book/ntb/ntb-e1.1/
author: PI
date: 2018-01-11 00:00:00 +0700
---
**Exercise 1.1**. Let $a,b,d \in \mathbb{Z}$ with $d \neq 0$. Show that $a \mid b$ if only if $da \mid db$.

**Solution**

$\forall a,b \in \mathbb{Z}$ and $a \mid b$

$\Leftrightarrow \exists \ z \in \mathbb{Z} : az=b$

$\Leftrightarrow daz=db, \forall d \neq 0 \in \mathbb{Z}$

$\Leftrightarrow da \mid db$

$\Rightarrow ~ \Box$
<br/><br/>

**Exercise 1.2**. Let $n$ be a composite integer. Show that there exists a prime $p$ dividing $n$, with $p \leq n^{1/2}$.

**Solution**

$\exists \ a,b \in \mathbb{Z} \ and \ 1 < a,b < n : ab = n, a \mid n, b \mid n $

$\Rightarrow$ if $a \leq n^{1/2}$ set $z = a$, if $a > n^{1/2}$, we have $b < n^{1/2}$ set $z = b$

$\Rightarrow \ \exists \ z \leq n^{1/2} \in \mathbb{Z} $ and $z \mid n$

$\Rightarrow$ if $z$ is a prime, set $p = z$, $p$ satisfies the requirements.

if $z$ is a composite $\exists \ p$ is a prime and $p \mid z$ and $p<z$. We have $ z \leq n^{1/2}$ and $z \mid n$ so $ p < n^{1/2}$ and $p \mid n$, $p$ satisfies the requirements.

$\Rightarrow ~ \Box$
	

