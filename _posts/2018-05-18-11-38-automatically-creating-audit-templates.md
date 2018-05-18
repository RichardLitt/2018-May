---
layout: post
title: "Automatically creating audit templates"
date: 2018-05-18T11:38:45Z
image: /assets/img/logo.png
---

I need a way to automatically update [my audit templates](https://github.com/mntnr/audit-templates) so that they pull down the most recent version, and automatically have some details filled in.

What I think I could do is:

```
curl https://raw.githubusercontent.com/mntnr/audit-templates/master/audit-template.md > audit-name.md
```

I think that's probably fine. But I don't want to have to continually remember the URL. I could add a line to my bash_profile... or perhaps an npm module? I could copy [covgen](https://github.com/simonv3/covenant-generator/blob/master/covenant.js)'s code pretty easily. Let's do that.