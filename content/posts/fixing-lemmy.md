---
title: "Why Lemmy/Kbin are fundamentally broken (and how to fix them)"
date: 2023-06-28T18:57:56-04:00
draft: false
---
This post assumes you have a basic understanding of what Lemmy and Kbin are.
Which, in turn, assumes you understand at least the concept of federation.

# The Issue
Currently, the way Lemmy/Kbin (which I will refer to simply as "Lemmy" for the rest of this article) work like this:

{{< rawhtml >}}
<img src="/instances.svg" style="filter:invert(1)"/>
{{< /rawhtml >}}

Cool, so our user can access content from both instances.
They go to Instance #1 to talk about transporation, and Instance #2 to talk about animals.
What could go wrong?

{{< rawhtml >}}
<img src="/instanceohno.svg" style="filter:invert(1)"/>
{{< /rawhtml >}}

Oh, no.

Now there exists *two* communities for the same topic!
No matter where our user posts, they'll be missing out on a portion of the audience!

And that's the issue. These instances decide they can have their own communities, and they turn inward.
They start to defederate.
And now, when a potential new user comes to join the platform, they're overwhelmed by the choices.
And instead of having one big community of connected instances, we have multiple redundant communities which aren't interacting at all!

## So how do we fix this?
This is where my proposal comes in.
You see, Reddit, a centralized platform, has subreddits for all topics.
So, when decentralizing Reddit, the natural move was to simply let each instance have it's own communities.

However, as we just saw, in practice, this wasn't the best of ideas. Lemmy even shows you posts from your own instance by default! (You have to switch to "All" to post with other instances).

This is definitely not ideal.

So let's try to fix this issue. What can we do?
Well, maybe we could add a tag to each community. Then, every post made from that community gets the tag.
With this system, it doesn't matter which community you post from, because instead of viewing posts from your community, you'd view all the posts that are tagged.

{{< rawhtml >}}
<img src="/instanceohyes.svg" style="filter:invert(1)"/>
{{< /rawhtml >}}

And this then begs the question; why even have communities? Now, the only purpose instances serve are for posting and moderating. You don't need the community anymore. Instead, just post straight to the tag itself.
{{< rawhtml >}}
<img src="/instanceohyeahhh.svg" style="filter:invert(1)"/>
{{< /rawhtml >}}

And that's it.

## Moderation

The only thing each instance is left to do is moderate. Each instance is responsible for two things:
- Moderating the content it puts out
- Moderating the content it receives

Say one rowdy user puts out some form of derogatory comment.
The instance from which this user posts has the authority to delete his post/comment.
In doing so, the instance also removes this post from all other instances.
Some may be worried about censorship. However, when you make your account on an instance, you give it a level of trust.
If you learn that you can't trust the instance, you can simply move to another one.

Of course, users could still just post from an unmoderated/personal instance. Hence, moderators are also responsible for moderating content put out by others. In this scenario, the content should simply be marked as hidden; the user still has the ability to view the comment/post, but only has to if they feel like it. (Content like this would also preferably be put at the bottom of comment chains).

## Parting Notes

And that's it! Of course, it's a big proposal(changes the core of Lemmy/Kbin at the fundamental level), but I really do believe it's what we need to make such a system work. I've always preferred the forum-style threads of Reddit to the posts of Twitter/Mastodon, so I really hope we can fix this system.

In the meantime, I've found myself using [Tildes](https://tildes.net) quite a bit. Although it's invite-only, the community is quite vibrant, the discussions are rich and meaningful, and the app itself is run by a non-profit. The UI is clean, and the site itself is snappy and just amazing to use(I actually much prefer it over Kbin/Lemmy).

Federation is a great idea, and I'd love to see it done right.
