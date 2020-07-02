Hey there! This is my cool thing that I built. Someday it might be a super cool full-stack app but for now it's mostly boilerplate.

# bootstrapping

You'll need the following repos in here to put together the app:

- git clone `https://github.com/jkachmar/example-cabal-project`
  - You may ignore all mention of `nix`.
  - Setup github actions with GHC 8.6.5 and the default version of cabal.
  - `sed -i '22d' example-cabal-project.cabal && cabal configure && cabal build` is sufficient to build this repo
- git clone `git@github.com:jared-w/hello-vue.git`

# contributing

My apologies, I'm still working on making this section easier.
For now there's a bit of manual setup required.

1. clone this repo, bootstrap the things.
2.

- `docker build -f Dockerfile.haskell example-cabal-project`
- `docker build -f Dockerfile.vue hello-vue`

And then you can run those without having to install a bunch of stuff to your laptop! Great!

# suggested reading

- https://github.com/actions/setup-haskell
- https://github.com/actions/setup-node
- https://help.github.com/en/actions/reference/software-installed-on-github-hosted-runners
- https://docs.github.com/en/actions/getting-started-with-github-actions
