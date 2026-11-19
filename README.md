## Guide to setting your git commit metadata emails

TLDR;

1. Find your github noreply email - This is written in [Settings -> Emails](https://github.com/settings/emails) and has the following format: `*****@users.noreply.github.com`
2. In that same Emails setting screen enable the `Keep my email addresses private` option, enabling this will show another option `Block command line pushes that expose my email` which we recommend to turn on as well to avoid pushing commits with private emails (this option will reject commits if you do not follow number 3).
3. Set you global mail config with github noreply email: `git config --global user.email "*****@users.noreply.github.com"`.
4. for certain private repositories that you want to share your private email because you want developers to have that extra communication you can set local config inside the repo directory with your private email: `git config user.email <private email connected to github>` but in that case you will have to turn off the option that we enabled in number 2: `Block command line pushes that expose my email`
