Heroku buildpack: Deep Thought
======================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) for use with [Deep Thought](https://github.com/redhotvengeance/deep_thought). If you need the ability to add a ssh key to your Heroku-hosted Deep Thought, then you've come to the right place.

This buildback is based on the [heroku/heroku-buildpack-ruby](https://github.com/heroku/heroku-buildpack-ruby) buildpack.

Usage
-----

Set the buildpack:

    heroku config:set BUILDPACK_URL=https://github.com/redhotvengeance/heroku-buildpack-deep-thought.git

Add your Deep Thought ssh key:

    ssh_key=`cat ~/.ssh/your_ssh_key`
    heroku config:set SSH_KEY="$ssh_key"

Additionally, add the domain where your repos are hosted:

    heroku config:set SSH_HOST=github.com

## Contribute

1. Fork
2. Create
3. Code
4. Test
5. Push
6. Submit
7. Yay!
