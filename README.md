# IronSKY × SIEM — Storage Log Forwarding (Amazon S3)

Beginner-friendly documentation site for feeding IronSKY (SecIron) mobile-RASP
event data from an Amazon S3 bucket into your SIEM.

**Live site:** https://fairuzlq.github.io/ironsky-siem-log-forwarding/

Covers: what SecIron provides (bucket, credentials, access), where the data lives
(path layout + `.json.gz` NDJSON format + fields), and the step-by-step SIEM side
(store credentials → AWS CLI → test access → `s3 sync` → extract/normalize →
feed into the SIEM → schedule → parse & detect), plus verification, troubleshooting,
and FAQ. Wazuh is used as the worked example; the approach is SIEM-agnostic.

Single self-contained `index.html` (no build step). All bucket names, APP_IDs, and
keys shown are placeholders — replace with the real values from SecIron.
