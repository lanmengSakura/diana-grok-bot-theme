# Security policy

## Public release boundary

This repository contains inert CSS, artwork, and documentation. It has no launcher or runtime injection path and does not by itself modify or start Grok Bot.

The verified local adapter is build-specific and uses renderer inspection over local loopback, so it remains private. Never publish that adapter, launch arguments, ports, process state, logs, screenshots, account/session material, credentials, or target-application binaries here. A successful CSS validation is not proof of a live mount.

## Compatibility

Every compatibility claim is tied to the exact version listed in `PRE_RELEASE.md`. Updates to the target application require a new verification pass before release.

## Reporting

Do not include private account or session material in a report. Use GitHub Security Advisories for vulnerabilities and ordinary Issues for non-sensitive compatibility defects.
