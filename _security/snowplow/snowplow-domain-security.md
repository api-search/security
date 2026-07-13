---
api_specs:
- filename: snowplow-console-api-openapi.yml
  format: yaml
  label: Snowplow Console API
  slug: snowplow-console-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snowplow/refs/heads/main/openapi/snowplow-console-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: snowplow.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: snowplowanalytics.com
  spf: true
hosts:
- cert_expires: Oct  3 22:52:10 2026 GMT
  host: snowplow.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 11:15:27 2026 GMT
  host: docs.snowplow.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: console.snowplowanalytics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Snowplow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Snowplow, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Snowplow
provider_slug: snowplow
slug: snowplow-domain-security
source_filename: snowplow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snowplow.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 22:52:10 2026 GMT\n  hsts: false\n- host: docs.snowplow.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 11:15:27 2026 GMT\n  hsts: false\n- host: console.snowplowanalytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: snowplow.io\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: snowplowanalytics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snowplow/refs/heads/main/security/snowplow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Analytics Platform
- Behavioral Data
- Data Collection
- Data Engineering
- Data Pipeline
- Event Tracking
- Open Source
---
