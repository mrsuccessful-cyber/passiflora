# Rosely Documentation

This contains the documentation of the [Rosely](https://github.com/hellotham/Rosely) design system, written in [Hugo](https://gohugo.io) using the [Docsy](https://github.com/google/docsy) theme.

It is currently hosted at [Netlify](https://netlify.com). The website address is https://rosely.hellotham.com

## Cloning the Project

The following will give you a project that is set up and ready to use (don't forget to use `--recurse-submodules` or you won't pull down some of the code you need to generate a working site). The `hugo server` command builds and serves the site. If you just want to build the site, run `hugo` instead.

```bash
git clone --recurse-submodules --depth 1 https://github.com/hellotham/rosely-docs.git
cd rosely-docs
npm install
hugo server
```

## Deployment with Netlify

Follow the instructions in *Host on Netlify* to set up a Netlify account (if you don’t have one already) and authorize access to your GitHub or other Git provider account. Once you’re logged in:

1. Click New site from Git.
2. Click your chosen Git provider, then choose https://github.com/hellotham/rosely-docs.git from your list of repos.
3. In the Deploy settings page:
    1. For your Build command, specify `cd themes/docsy && git submodule update -f --init && cd ../.. && hugo`. You need to specify this rather than just hugo so that Netlify can use the theme’s submodules.
    2. Click Show advanced.
    3. In the Advanced build settings section, click New variable.
    4. Specify `HUGO_VERSION` as the Key for the new variable, and `0.79.1` or later as its Value.
    5. (Optional) Click New variable again, and this time set `HUGO_ENV` to `production`. Do this if you want your site to be indexed by search engines. You must do this if you want to use a Google Custom Search Engine.
4. Click Deploy site.

Alternatively, you can follow the same instructions but specify your Deploy settings in a netlify.toml file in your repo rather than in the Deploy settings page. You can see an example of this in the Docsy theme repo.

If you have an existing deployment you can view and update the relevant information by selecting the site from your list of sites in Netlify, then clicking Site settings - Build and deploy. Ensure that Ubuntu Xenial 16.04 is selected in the Build image selection section - if you’re creating a new deployment this is used by default. You need to use this image to run the extended version of Hugo.