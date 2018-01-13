---
layout: post
creationdate:  2018-01-05 00:00:00 +0700
title: Dvisibility and primality
permalink: /book/ntb/ntb1.1/
author: PI
date: 2018-01-10 00:00:00 +0700
---

The integers $\mathbb{Z}=\\{...,-2,-1,0,1,2...\\}$.

$a,b,z \in \mathbb{Z}$ \\
$az=b $ \\
We say that: \\
$a$ **devides** $b$. Write $a \mid b $.\\
$a$ is a  **divisor** of $b$, or $b$ is a **multiple** $a$, or $b$ is  **divisible** by $a$. \\
If $a$ does not devide $b$, then we write $a \nmid b$.

**Theorem 1.1**. $a,b,c \in \mathbb{Z}$.\\
	1. $a \mid a$, $1 \mid a$, and $a \mid 0$;\\
	2. $0 \mid a$ if and only if $a=0$;\\
	3. $a \mid b$ if and only if $-a \mid b$ if and only if $a \mid -b$;\\
	4. $a \mid b$ and $a \mid c$ implies $a \mid (b+c)$;\\
	5. $a \mid b$ and $b \mid c$ implies $a \mid c$;

**Theorem 1.2**. For all $a,b \in \mathbb{Z}$, we have $a \mid b$ and $b \mid a$ if and only if $a \pm b$. In particular, for every $a \in \mathbb{Z}$, we have $a \mid 1$ if and only if $a = \pm 1$.

**Theorem 1.3 (Fundemental theorem of arithmetic)**. Every non-zeo innteger $n$ can be expressed as
<span style="text-align: center; display:block;"> $$n = \pm p_{1}^{e_{1}} ... p_{r}^{e_{r}} $$</span>
where $p_{1},...,p_{r}$ are distinct primes and $e_{1},...,e_{r}$ are positive integers. Moreover, this expression is unique, up to a reordering of the primes.

**Theorem 1.4 (Division with remainder property)**. Let $a,b \in \mathbb{Z}$ with $b>0$. Then there exist unique $q,r \in \mathbb{Z}$ such that $a=bq+r$ and $0 \leq r < b$.

**Theorem 1.5**. Let $a,b \in \mathbb{Z}$ with $b > 0$, and let $x \in \mathbb{R}$. Then there exist unique $q,r \in \mathbb{Z}$ such that $a=bq+r$ and $r \in [x,x+b)$.
