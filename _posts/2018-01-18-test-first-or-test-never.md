---
layout: post
title:  "Test first, or test never"
categories: testing tdd test-first
published: false
---
> If you don't write the tests before you write the corresponding production code, you might as well never write the tests at all.

The idea of writing and having automatic tests has come a long way in our industry. Everywhere I go, developers have heard of it and they generally think it's a good thing to do. Most even do it, at least to some extent and at least every now and then. On the surface, this would seem like a good thing. But on the contrary, I believe this indifference toward writing tests is destructive for our industry. Because the thing is, like with so many other systems and methods - if you apply it half-heartedly, you will pay the price but not reap the benefits.

My claim therefore, is this: **If you do not believe writing tests is a time-saving, quality-heightening and generally value-adding best practice that should be applied on every piece of production code - then you probably have never seen it done properly.**

One of the most common objections to spending a lot of energy on writing good tests, goes something like this:

> But how can we test the tests? Why bother with testing the production code, if we cannot test the tests?

I used to be taken off guard by this or similar questions, but after taking a step back and pondering a bit, it has become utterly clear to methen it became clear to me: We are in fact testing the tests by writing them _before_ the production code so that **they fail when we first write them**. This last part cannot be stressed enough, and is the entire point of this post.

To illustrate this, let me walk you through two different scenarios: one where we write the test first, when it fails, and another where we write the test after the fact, simply to support the production code we have already built. 
