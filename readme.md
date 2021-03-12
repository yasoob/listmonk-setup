# Listmonk production setup example

Hi people! 👋 This repo is just an example of how you can potentially set up [listmonk](https://github.com/knadh/listmonk) in production. This setup adds SSL support to listmonk. I have written an extensive guide on [how to setup listmonk](https://yasoob.me/posts/setting-up-listmonk-opensource-newsletter-mailing/). It might be helpful to read that before cloning this repo.

### ⚙️ Configuration

You need to make a few changes before using the code in this repository. 

1. `init-letsencrypt.sh`

    - Add your custom domain in line 8
    - Add your email address in line 11

2. `config.toml`

    - Change the admin user & pass on line 9 and 10

3. `data/nginx/nginx.conf`

    - Replace all occurances of `example.com` with your domain

### 🚀 Installation & Launch

Run `init-letsencrypt.sh` to get the certificates set up. It will also start listmonk during the process.
