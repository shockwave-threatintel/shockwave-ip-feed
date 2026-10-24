# Shockwave IP Threat Intelligence Feed

Shockwave is a community threat-intelligence project providing IP indicators to support defensive security operations.

The initial release candidate is a community IPv4 indicator feed derived from data published under terms permitting reuse. Inclusion does not mean that Shockwave has independently confirmed malicious activity for every address.

## Dashboard

The planned public dashboard will provide release information, feed statistics and access to the published feed once the initial release has been approved and deployed:

https://shockwave-threatintel.github.io/shockwave-ip-feed/

## Initial feed

- **Format:** Plain text, one IPv4 address per line.
- **Initial candidate:** 613 unique public IPv4 addresses in the current release candidate.
- **Duplicates:** Removed during feed processing.
- **Address validation:** The current candidate passed IPv4 format, uniqueness and public-address checks.
- **Evidence level:** Community-reported indicators; individual entries have not all been independently investigated or corroborated by Shockwave.

The candidate count is not a claim that every entry is currently malicious, nor does it measure the accuracy of the underlying indicators.

## Feed methodology and use

The current release candidate uses a community threat-intelligence feed with a rolling time window. Shockwave validates IPv4 addresses, excludes non-global addresses and removes duplicates. These checks do not independently verify every indicator or guarantee that an address is currently malicious.

The feed is intended for defensive security use. Consumers should assess indicators in their own environments and consider monitoring or alerting before enforcing blocking rules. The feed is provided without a guarantee that every indicator is accurate or remains relevant. Consumers are responsible for checking the applicable terms before redistributing or using the data.

## Intended use

The feed is intended to support defensive security activities, including:

- Threat hunting and security analysis.
- Firewall and network-security monitoring.
- Security information and event management.
- Carefully evaluated IP reputation controls.

**Recommended deployment:** Begin in monitoring or alert-only mode. Evaluate the indicators against local traffic and trusted infrastructure before considering enforcement.

Do not deploy the feed as an unconditional block rule without testing. Monitor false positives, maintain an allowlist and provide a rollback procedure.

## Understand the limitations

Shockwave combines indicators from third-party threat-intelligence sources with independent validation and reputation cross-checks. Best-effort verification is performed using available external intelligence and retained assessment evidence, with findings evaluated separately from release decisions.

These checks improve the evidence available for each indicator, but they do not guarantee that every IP is malicious or that an address remains a threat at the time it is used. IP addresses can be reassigned, shared by legitimate services, or associated with compromised infrastructure. False positives and stale indicators remain possible.

Shockwave recommends monitoring or alert-only deployment first, followed by local validation and careful review before enforcement.

## Publication and maintenance

Releases are reviewed before publication. The public release status and feed statistics are maintained separately from the feed-generation process.

The project should publish a new release only after the candidate has been validated, reviewed and approved. Release-to-release additions and removals should be reported when a previous public release exists and a comparison has been performed.

## Responsible use

Shockwave is provided for defensive security and threat-intelligence purposes. Consumers are responsible for complying with applicable laws, source licensing and their own operational requirements.
