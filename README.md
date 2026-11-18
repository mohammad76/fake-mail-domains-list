# Disposable email domains

`fake-mail-domains-list.txt` contains one ASCII domain per line. It is a snapshot of the [disposable-email-domains blocklist](https://github.com/disposable-email-domains/disposable-email-domains/blob/main/disposable_email_blocklist.conf), published under [CC0 1.0](https://github.com/disposable-email-domains/disposable-email-domains/blob/main/LICENSE.txt).

The snapshot from 2026-11-18 contains 10,400 domains. It replaces the older aggregate, which included permanent providers such as `protonmail.com`.

To refresh, download the upstream file to a temporary path, check the diff, and confirm that known disposable providers such as `mailinator.com` are present and that permanent providers such as Gmail and Proton Mail are absent. Replace the snapshot after validation and publish it through the normal repository workflow. Hub downloads this file on deployment and has a bundled copy for offline use.
