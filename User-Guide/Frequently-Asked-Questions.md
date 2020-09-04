### Frequently asked questions about Greentea OS project

> **Hint:** Hover on the point and click on the appearing "link" icon to share answers to questioners

#### What is Greentea OS, shortly?

Greentea is a free next-generation operating system for your PC

#### Is Greentea OS an operating system, distro, visual theme or app?

Similiar to macOS and Linux, Greentea is a full operating system, installable on a PC. It runs apps, games and has some built-in software.
It is **not** based on any other system.

#### Is Greentea OS Ad-driven or funded by corporations?

Nope. Greentea is funded solely by [donations](https://greenteaos.github.io/donate/).

#### Is Greentea OS a GNU/Linux distro?

No. It is an independent OS, without Linux kernel.

#### What makes Greentea OS so unique?

***From developer perspective:*** runtimes-based OS, aimed at strict isolation, it has no API to itself from user space.
To achieve those goals, we created new kernel for it — Tofita.

***From user perspective:*** apps cannot break the system or make it slow. System updates are fast and not annoying.

Being internally very different from common ones,
this system is friendly and does not push "innovations" at you face, thus making you feel at home.

[More info about what makes Greentea so special](https://github.com/GreenteaOS/Greentea/blob/master/README.md#what-makes-greentea-so-special)

#### How to track the progress in real time?

Visit [our Trello board](https://trello.com/b/zIHcmPnB) and check commits history of GitHub repos.

#### What is Tofita?

[Tofita](https://github.com/GreenteaOS/Tofita) is *the* Greentea OS kernel, the core, the heart of the system.

#### Where I may download it?

We don't provide public builds yet, only for developers and testers.

#### How can I test it?

Check our [Telegram group](https://t.me/greenteaos) and ask for builds or [download manually](https://ci.appveyor.com/project/PeyTy/tofita/build/artifacts).

#### Is it safe to host this project on GitHub?

Yes. Git is a system, on which GitHub is based, used to store and operate on project's source code.

Git is **distributed**, **decentralized** and **consistent**. It is **not** possible to silently edit, hack or fake code.

There is no reason to worry about.

#### I've seen some "fake" commits. Are fake commits a thing?

Sadly, GitHub, as any other service, has small bugs in it. The bug may **visualize** fake commits, but fakes cannot be committed into project itself! So no real code touched, albeit it looks "hacked". Also, Git, as a system, allows to set arbitrary committer names, so they sould not be considered 100% real without "Verified" badge on them.

That being said, you should not follow misleading information with fake links.

#### What application compatibility is going to be supported?

We support only classic-style APIs.

#### Is Greentea made specifically for modern hardware?

Greentea builds for comparatively modern hardware only — approximately for most PCs made in the last 10+ years, counting from 2009.

The oldest hardware with possibility to run is 2007 (64-bit CPUs only), but this is not guaranteed.

### Sometimes Greentea definitely looks familiar...is this intentional?

We investigate design decisions of Linux and Android.

Note, that the *only* desktop things we try to keep are a flat look of window frames, sharp user interface edges and
basics like font & icon sizes (for app compatibility and user experience familiarity).
And drawing rectangles seems to give better performance than rounded corners.
