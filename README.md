# CUBE CSS with Tailwind CSS

⚠️ **THIS IS VERY MUCH A PROTOTYPE AND LIKELY BROKEN** ⚠️

**Attention:**  
_A challenge for me in this project is that if we’re going to run with this approach, it’s looking we can’t really use Sass, which I am a fan of for keeping my CSS nice and organised. The way I see it though is that you need to meet each other in the middle in these situations, so I’ll pass-up Sass, just like the other developers are passing-up using Tailwind for everything._

_What I want to really avoid is the PostCSS pretending to be Sass setup—which is very possible—but oh-so-fragile. I’ve had awful experiences with this too. Instead, I’ll be recommending that we lean into CSS Custom Properties. We could use Tailwind’s @apply to apply utilities in our components (Blocks in CUBE CSS), but that in my opinion is some potentially expensive technical debt. Mainly because I can already see issues with how Tailwind might clash with upcoming CSS features, such as @layer._

_In the space of very little time, I managed to roll-out a little generator that takes Tailwind config groups and generates CSS Custom Properties. This is a good start and could rather easily create a solid system for creating reusable tokenised CSS—even if—or even, when—Tailwind is no longer preferable to the wider team._  
Source: https://piccalil.li/blog/i-used-tailwind-for-the-u-in-cube-css-and-i-liked-it/

An example of how you can use [Tailwind CSS](https://github.com/tailwindlabs/tailwindcss) as the U (utilities) in
[CUBE CSS](https://cube.fyi/). It also uses the following:

1. [Every Layout](https://every-layout.dev/) layouts as compositional layouts (the C in CUBE CSS)
2. [Utopia](https://utopia.fyi/) for fluid type and spacing scales
3. [Post CSS](https://postcss.org/) to bundle up CSS files

## Why?

I work with clients that like to use Tailwind and I, as part of the
consultancy work I do, try to encourage them down the path of a CSS
methodology, rather than leaning all-in on a CSS framework.

Tailwind is _fantastic_ at generating utility classes with an
easy-to-understand config file, but I find it very limiting and rigid as the
entire CSS codebase, so this project uses it how I would ideally use it:
purely as the utility generator.

Consider this project diplomacy.

## Getting started

1. Run `npm install`
2. Run `npm start` to spin up a little local server and watch for CSS changes
3. Run `npm build` to compress CSS etc

## Contributing

No thanks, but if you see something fundamentally wrong (not just your
opinions, thanks), then let me know in the issues!
