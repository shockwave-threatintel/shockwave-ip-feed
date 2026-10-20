# Shockwave IP Threat Intelligence Feed

Shockwave is a community-facing threat-intelligence project that provides a publicly accessible feed of IP addresses associated with malicious activity.

The feed is intended for security teams, network administrators and defensive security systems. It will also be used within our own security environment, subject to validation and operational testing.

## Dashboard

The initial read-only dashboard interface is available in [index.html](./index.html). It is a dashboard scaffold, not yet a live hosted website. It shows an unpublished state until an approved release-status file is provided.

## Inclusion policy

Shockwave follows a conservative, high-confidence approach.

IP addresses are considered for inclusion when credible threat intelligence or corroborating evidence supports their association with malicious activity. Suspicious behaviour alone is not automatically sufficient.

The project aims to:

- Prioritise credible evidence over feed size.
- Validate and deduplicate entries before publication.
- Exclude private, reserved and otherwise unsuitable IP address ranges.
- Review conflicting or insufficient evidence before inclusion.
- Avoid presenting uncertain indicators as confirmed threats.

## Feed format

The planned public feed will use a plain-text format containing one IPv4 address per line.

- Duplicate entries will be removed.
- Entries will be validated before release.
- The public feed URL and update information will be documented once the publication process is finalised.

## Intended use

The feed may be used to support defensive security controls, including firewall policies, threat hunting, monitoring and security analysis.

Consumers should evaluate the feed against their own security requirements and operational context before deploying blocking rules.

**An IP address appearing in Shockwave is an indicator for investigation or defensive action, not proof that every connection involving that address is malicious.**

IP addresses can be reassigned, shared by multiple services, or associated with legitimate infrastructure. False positives are possible.

## Publication and maintenance

Releases will be reviewed and published manually.

Before a release, the feed should undergo validation for address format, duplicates, unsuitable ranges and release integrity. Publication should occur only after the candidate feed has been reviewed and approved.

The project will document its publication process and update information as these are established.

## Responsible use

Shockwave is provided for defensive security and threat-intelligence purposes. Consumers are responsible for assessing the suitability of the feed for their environment and for monitoring the effects of any controls based on its contents.

The project does not guarantee that every indicator is correct, current or suitable for automatic blocking.

## Project status

The dashboard scaffold has been committed, but no public threat feed has been released. The feed should not be considered production-ready until its contents and publication process have been validated.
