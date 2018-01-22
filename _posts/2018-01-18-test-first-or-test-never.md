---
layout: post
title:  "Test first, or test never"
categories: testing tdd test-first
published: true
---
> If you don't write the tests before you write the corresponding production code, you might as well never write the tests at all.

The idea of writing and having automatic tests has come a long way in our industry. Everywhere I go, developers have heard of it and they generally think it's a good thing to do. Most even do it, at least to some extent and at least every now and then.

One of the most common objections to spending a lot of energy on writing good tests, is this:

> But how can we test the tests?

I used to be taken off guard by this or similar questions, but after taking a step back and pondering a bit, it has become utterly clear to methen it became clear to me: We are in fact testing the tests by writing them _before_ the production code so that **they fail when we first write them**. This last part cannot be stressed enough, and is the entire point of this post.

To illustrate this, let me walk you through two different scenarios: one where we write the test first, when it fails, and another where we write the test after the fact, simply to support the production code we have already built. 
