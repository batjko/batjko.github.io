---
published: true
---
## Goodbye Angular

So it looks like I joined my new company just in time: Our little Apps team is in this envying position where there are a number of vague projects on the horizon, but no deadlines and no actual requirements exist yet. So we decided to take a week or two off from sprints and instead evaluate what Front-End frameworks we actually want to be developing those future projects in. Withoiut any pressing projects or a large amount of pre-existing legacy code base, now is the perfect time to be shopping around.

There has been some Angular 1 knowledge circulating in the team, with one or two minor apps having been done that way (I worked on one for my first month at this company). But I am happy to note that there was no debate about my suggestion to re-evaluate now. Both my team mates and our boss are fully on board. Certainly not the kind of response I was used to in my old corporate job.
"So", I thought, "...let's play."

## The World is Our Oyster!

Almost immediately, we dismissed comparatively minor frameworks such as Aurelia, Vue and Ember. We want long-term backing (whatever that means these days) by a major player and a large community for secondary resources as one of the basic requirements. Essentially, we didn't want to be left havign to maintain an outdated and underdocumented stack after 6 months. That condition alone really only left Google's Angular 2 and Facebook's React for a closer examination.

We investigated Angular 2 and although it has some merit, most notably the focus on componentisation and strong community support, Facebook's already had both for years, has matured greatly by now and - most importantly - people *still* love it! In fact, its popularity is still growing exponentially.
The same can certainly not be said of Angular 2, even a week after its official release (granted, the alphas, betas and RCs have been out for quite a while, with uninterrupted churn of breaking changes): 

1. Its detractors don't like that it is jamming Typescript down our collective throats.
2. Dependency Injection is still a bloody mess (and yet they celebrate it as a major selling point)!
3. Somewhat overzealous adoption of Javascript features that are barely past the proposal stage (not that I dislike decorators, but it's a bit early to make them a major feature of your Production-ready framework)
4. Google aren't even dogfooding their own framework!
5. It still wants to own the whole app, bullying everything non-core to be wrapped into an Angular service.
6. Despite pushing Ecmascript boundaries (bold move), their component model is pretty much locked into classes, sticking with a certain preference for OOP.

## Take me right here, React!

I'd imagine React's responses to the above issues might go along these lines:

1. Use ES5, use Babel for ES6+ or transpile from Dogescript... React don' care.
2. Just require or import what you need, Javascript style. We kinda recommend the way Node already does it.
3. You should use ES6, but it all works just fine in ES5 and we are happy to show you both!
4. React is used in the most critical of Facebook's front-end apps, including Instagram and the their mobile apps (React Native).
5. npm.   Just import and use.
6. We heard you like functional programming, so we put functions into your functional components. ;)

The illuminating quote that decided the issue for me, was this:

> Learn Angular to become a great *Angular* developer.
> Learn React to become a great *Javascript* developer.

So, while we acknowledge Angular 2's powerful features and capabilities that it comes with out of the box, its strongly opinionated approach ultimately wasn't what we wanted to be developing with for the next few years.
Thus, we decided to leave Angular's socialism behind, in favor of React's libertarianism.

On we went to explore the React ecosystem:

* Turns out Redux actually does make a lot of sense, after all. Planning a single state for your app is a challenge, though. I even tweeted His Redux Highness, Dan Abramov himself, for advise on design considerations for a Redux app, but even he couldn't help me out. This could be improved, eco-system!
* Webpack is complicated, but freaking awesome! ...Get the hell off me, dirty Gulp!
* Enzyme's simplicity is ideal for starting out with testing React components. And Mocha, obviously.

Now, I could probably convince the team to adopt the Airbnb style guide for React. But will they let go of their semicolon prejudices and switch to StandardJS, I wonder? ;)
