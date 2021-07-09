# 🩺 Alleviam

This is Alleviam, the Early Detection Research Network [EDRN](https://edrn.nci.nih.gov/) alleviation and monitoring system. Alleviam keeps tabs on essential informatics services, files tickets when things are not copacetic, and keeps the EDRN (and related projects) up and running as much as possible.

## 🏃‍♀️ Getting Started

Check the documentation for [Upptime](https://upptime.js.org/) first. Then do a `git pull` because the [GitHub Actions](https://github.com/features/actions) that powers this make numerous commits to the repository. Then edit the `.upptimerc.yml` file and commit and push.

You can then view the results at https://edrn.github.io/alleviam/ (powered by [GitHub Pages](https://pages.github.com)).

As systems go down, [issues are automatically filed and assigned](https://github.com/EDRN/alleviam/issues) (powered by [GitHub Issues](https://docs.github.com/en/issues/tracking-your-work-with-issues/about-issues)).

Email notifications are set up, but haven't been tested. Future notification options such as text messages should be explored later.


### 🤫 Secrets

The following [repository secrets](https://github.com/EDRN/alleviam/settings/secrets/actions) are in use:

-   `GH_PAT`: a personal access token with `repository` and `workflow` scopes so Alleviam can run
-   For DMCC Password Verification tests:
    -   `DMCC_USERNAME`: a valid "EDRN Secure Site" username
    -   `DMCC_PASSWORD`: the matching valid password for the given "EDRN Secure Site" username
-   For Directory Service tests:
    -   `MCL_BASIC_AUTH`: a base-64 encoded HTTP Basic authentication value containing the MCL `service` account username and password
-   For email notifications:
    -   `NOTICATION_EMAIL`: the value `true` to tell Upptime we want emails
    -   `NOTICATION_EMAIL_FROM`: a source email address
    -   `NOTIFICATION_EMAIL_TO`: the destination email address to notify; this is currently a single user (Sean Kelly) for testing purposes, but should be set to a group account in the future
    -   `NOTIFICATION_EMAIL_SENDGRID`: the value `true` to tell Upptime to use [Sendgrid free account](https://sendgrid.com) for email transmission
    -   `NOTIFICATION_EMAIL_SENDGRID_API_KEY`: the API key to a Sendgrid account



## 🖥 The Software

This effort is based on [Upptime](https://upptime.js.org/).

## 🔢 Versioning

We'll use the [SemVer](https://semver.org/) philosophy for versioning of this software.

## 👥 Contributing

You can always look at [open issues](https://github.com/EDRN/alleviam/issues) and/or make [pull requests](https://github.com/EDRN/alleviam/pulls).

## 📃 License

The project is licensed under the [Apache version 2](LICENSE.md) license.
