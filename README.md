# Shockwave IP Threat Intelligence Feed

Shockwave is a community threat-intelligence project that aggregates publicly available IP indicators to support defensive security operations.

The initial release is an **aggregated community blocklist** containing IPv4 addresses collected from multiple threat-intelligence sources. Inclusion in this feed does not mean that Shockwave has independently confirmed malicious activity for every address.

## Dashboard

The planned public dashboard will provide release information, feed statistics and access to the published feed once the initial release has been approved and deployed:

https://shockwave-threatintel.github.io/shockwave-ip-feed/

## Initial feed

- **Format:** Plain text, one IPv4 address per line.
- **Initial candidate:** 16,484 unique public IPv4 addresses in the current release candidate.
- **Duplicates:** Removed during aggregation.
- **Address validation:** The current release candidate passed IPv4 format, uniqueness and public-address checks.
- **Evidence level:** Aggregated source indicators; individual entries have not all been independently investigated or corroborated by Shockwave.

The candidate count is not a claim that every entry is currently malicious, nor does it measure the accuracy of the underlying sources.

## Sources and aggregation

Shockwave Threat Intelligence aggregates indicators from multiple threat-intelligence inputs into a consolidated IPv4 feed.

The aggregation process validates IPv4 addresses, excludes non-global addresses and removes duplicates. These checks do not independently verify every indicator or guarantee that an address is currently malicious.

The feed is intended to remain freely accessible and is not offered for resale. Consumers are responsible for assessing indicators before applying security controls and for ensuring their use of the feed is appropriate for their environment.

To protect upstream relationships, source identities and source-specific information are not publicly disclosed.

## Intended use

The feed is intended to support defensive security activities, including:

- Threat hunting and security analysis.
- Firewall and network-security monitoring.
- Security information and event management.
- Carefully evaluated IP reputation controls.

**Recommended deployment:** Begin in monitoring or alert-only mode. Evaluate the indicators against local traffic and trusted infrastructure before considering enforcement.

Do not deploy the feed as an unconditional block rule without testing. Monitor false positives, maintain an allowlist and provide a rollback procedure.

## Limitations

IP addresses are not permanent identities. They can be reassigned, shared by legitimate services, used by cloud infrastructure or associated with compromised systems without every connection being malicious.

False positives and stale indicators are possible. Shockwave does not guarantee that every entry is accurate, current or suitable for automatic blocking.

Consumers are responsible for evaluating the feed and monitoring the impact of controls that use it.

## Publication and maintenance

Releases are reviewed before publication. The public release status and feed statistics are maintained separately from the feed-generation process.

The project should publish a new release only after the candidate has been validated, reviewed and approved. Release-to-release additions and removals should be reported when a previous public release exists and a comparison has been performed.

## Responsible use

Shockwave is provided for defensive security and threat-intelligence purposes. Consumers are responsible for complying with applicable laws, source licensing and their own operational requirements.
