# Code Graph direction

We have teams working on [Search](./search/index.md), [Code Insights](./code-insights/index.md), [Code Intelligence](./code-intelligence/index.md), and [Batch Changes](./batch-changes/index.md); this page describes the overarching mission and strategy that ties them together, but each linked team also provides a more detailed direction page with what they are working on next and why. There is also a whole-company [Sourcegraph direction](../index.md) available.

## Mission

We want to make finding, understanding, and editing code easier, regardless of how much you have, how complex it is, where you store it, or even how technical you are.

## Vision

### One year vision

> We want to ensure that we are solving the most critical problems for our enterprise users, focusing on retaining existing and acquiring new enterprise customers. By providing as much value as possible to them, we can grow the business while solving the hardest scaling and complexity problems for everyone.

### Three year vision

> We imagine a much more connected experience, not just in terms of the kinds of searching that you're able to do, but in how we can offer suggestions for interesting searches and what you can do with the results. Expanding on capabilities we've introduced recently, such as semantic search, insights, and batch changes, we will offer an unparalleled solution for searching and making decisions across branches, repositories, and even code hosts, beyond even what's possible today.

### Ten year vision

> We want to make using Sourcegraph to understand and modify code so easy that anyone can do it, including people not traditionally considered developers. We want to [democratize coding](../../company/strategy.md#10-year-vision) by making it so that everyone in the company can engage with the organization's code, safely making changes to implement their department's priorities and interests, without need for an intermediary to do it for them.

## Principles

### Abstraction vs. complexity

According to [The Case for 'Developer Experience'](https://future.a16z.com/the-case-for-developer-experience/) (by [Jean Yang](https://twitter.com/jeanqasaur)), there are two ways to think about categories of developer tools or features today:

- Abstraction tools, which simplify tasks away by providing building blocks, sane defaults, and frameworks to build on. Most existing developer tools are of this variety.
- Complexity-exploring tools, which help with complex problems such as finding and fixing issues in existing, heterogeneous software systems. I.e., ones that were created using the existing tools developers use today, with different languages, frameworks, and versions in constant flux, all interacting with each other.

This emerging need for complexity-exploring tooling is one we see Sourcegraph playing an important role in. "The reality is that software tech stacks today look more like a rainforest — with animals and plants co-existing, competing, living, dying, growing, interacting in unplanned ways — than like a planned garden" ([_The Case for 'Developer Experience' by Jean Yang_][1]), and we are mindfully designing our user experience to let you embrace this complexity rather than hiding it, or pushing you towards a specific single solution.

Practically, this means a few things as we think about how our product should work:

1. Sourcegraph fits in to your existing ecosystem – wherever you host your code, whatever language it's in, or however many repos you use.
1. By surfacing relationships (not just code itself, but data types, configuration, and more) we help you build a clear, meaningful model of your software.
1. We make this information easy to explore by revealing complexity as needed, with the most relevant information up front, easy to understand, and easy to share.

If we achieve these points, we can make it easy for developers to get things done and, ultimately, ship great code.

[1]: https://future.a16z.com/the-case-for-developer-experience/

## Themes

We are focused on several themes to help make our one year vision a reality. They are not listed in priority order, as we are pursuing all of them. To see how these play into what any particular product area is delivering, take a look at the individual team direction pages linked at the [top of this page](#code-graph).

### Make the power of our features easier to find and use

Learning what's possible and how to get the most out of our product tends to be trial and error, especially for an individual developer who might have a unique set of use cases and interests for which they would benefit from exploring. Making onboarding and interaction easier also helps our users and sales teams demonstrate the value of our product more quickly than is possible today.

### Level up our enterprise-ready features

How our product works in terms of pricing, upgrade paths, auditing, single sign-on, access control, and so on are essential for enterprise customers with large, complex organizations. In partnership with our Cloud team, we're focused on ensuring that these elements of our product meet and exceed these needs so that when it comes to rolling out Sourcegraph the logistics of getting set up don't get in the way of realizing the value of Big Code search.

### Deliver a unified experience

Our product solves real problems today, but investing in the polish, user experience, and cross-feature functionality within our product area to make the experience lovable and help us deliver solutions that are more than the sum of the parts. Code insights can lead you to a more detailed search, from which you might launch a more advanced semantic analysis. From here, you might use batch changes to remediate a problem and then document everything you've done in a search notebook. This flow works today, but we can do more to connect these experiences in ways that deliver more value than engaging with them separately.

### Scale for Big Code

We have more and more large customers dealing with a lot of code and complexity at scale. It's important that our platform meets their needs, not just in terms of search performance, but in allowing you to explore and understand complex interrelationships of meaning in source code, at the [world's largest scale](../../company/strategy.md#big-code).
