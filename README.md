# This is Noe Nieto's Resumé

This site was made with Jekyll using the [modern-resume-theme](https://github.com/sproogen/modern-resume-theme).

This repo has github actions to deploy this repo automatically to my site. I
used [lemonarc/jekyll-action](https://github.com/helaili/jekyll-action) to build
the site and [Pendect/action-rsyncer](https://github.com/Pendect/action-rsyncer)
to upload the changes to the server.


# Setup guide

This is mostly for a future me in case I don't remember how to set this up again (e.g. new laptop).

First, install bundler.

For fedora:

```bash
sudo dnf install rubygems ruby-devel redhat-rpm-config gcc-c++
```

On Debian 10.9 I did:

```bash
sudo apt install ruby ruby-dev bundler
```

Now run bundler:

```bash
bundle install
```

> [!NOTE]
> If you have problems with some gem version, try deleting the `Gemfile.lock` file and run `bundle install` again.


# Updating the resume

```bash
./dev watch
```

# Building the resume

```bash
./dev build
```

# Deploy
```bash
./dev deploy
```

Aaand, that's it.