---
api_specs:
- filename: overview
  format: yaml
  label: Airbridge API
  slug: airbridge-api
  spec_type: Postman
  url: https://www.postman.com/airbridge-engineering/workspace/airbridge-api/overview
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: airbridge.io
  note: No SPF record on the apex — the only TXT records are a Salesforce verification token and two Google site-verification tokens. DMARC exists but at p=none, which monitors without enforcing.
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ab180.co
  note: DMARC reporting addresses point at an individual mailbox rather than a role address.
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:amazonses.com include:sendgrid.net ~all
hosts:
- cert_expires: Oct 26 07:06:17 2026 GMT
  host: www.airbridge.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 10:29:10 2026 GMT
  host: help.airbridge.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: api.airbridge.io
  hsts: false
  hsts_max_age: null
  https: true
  note: The API host itself sends no Strict-Transport-Security header, although the docs state all requests must be made over HTTPS.
  tls_version: TLSv1.3
- cert_expires: Feb 21 23:59:59 2027 GMT
  host: mcp.airbridge.io
  hsts: false
  hsts_max_age: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: app.airbridge.io
  hsts: false
  hsts_max_age: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: sdk-download.airbridge.io
  hsts: false
  hsts_max_age: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 17:27:34 2026 GMT
  host: status.airbridge.io
  hsts: true
  hsts_max_age: 259200
  https: true
  note: Atlassian Statuspage-hosted.
  tls_version: TLSv1.3
- cert_expires: Nov 30 02:17:58 2026 GMT
  host: www.ab180.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 8
kind: domain-security
layout: security
method: probed
name: Ab180 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ab180, probed live across 8 host(s) and 2 registrable domain(s). 8 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Ab180
provider_slug: ab180
slug: ab180-domain-security
source_filename: ab180-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: 'live DNS/TLS/HTTP probes of every host in apis.yml plus the MCP, dashboard,\n  status and SDK-distribution hosts; baseline written by 0-working/probe-domain-security.py\n  and extended by hand-probed hosts the script did not derive'\nchecked: '2026-09-05'\nhosts:\n- host: www.airbridge.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Oct 26 07:06:17 2026 GMT'\n  hsts: true\n  hsts_max_age: 63072000\n- host: help.airbridge.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Nov 24 10:29:10 2026 GMT'\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.airbridge.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Feb 25 23:59:59 2027 GMT'\n  hsts: false\n  hsts_max_age: null\n  note: 'The API host itself sends no Strict-Transport-Security header, although the docs\n    state all requests must be made over HTTPS.'\n- host: mcp.airbridge.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Feb 21\
  \ 23:59:59 2027 GMT'\n  hsts: false\n  hsts_max_age: null\n- host: app.airbridge.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Jan 31 23:59:59 2027 GMT'\n  hsts: false\n  hsts_max_age: null\n- host: sdk-download.airbridge.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Jan 31 23:59:59 2027 GMT'\n  hsts: false\n  hsts_max_age: null\n- host: status.airbridge.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Oct  7 17:27:34 2026 GMT'\n  hsts: true\n  hsts_max_age: 259200\n  note: Atlassian Statuspage-hosted.\n- host: www.ab180.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Nov 30 02:17:58 2026 GMT'\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: airbridge.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n  note: 'No SPF record on the apex — the only TXT records are a Salesforce verification\n    token and two Google site-verification tokens. DMARC exists but at p=none, which\n    monitors without\
  \ enforcing.'\n- domain: ab180.co\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:_spf.google.com include:amazonses.com include:sendgrid.net ~all'\n  dmarc: true\n  dmarc_policy: none\n  note: 'DMARC reporting addresses point at an individual mailbox rather than a role\n    address.'\nfindings:\n- 'No CAA record on either registrable domain — any CA may issue for airbridge.io and\n  ab180.co.'\n- 'No DNSSEC on either domain.'\n- 'airbridge.io publishes no SPF record at all, while ab180.co does.'\n- 'Both DMARC policies are p=none, so neither enforces.'\n- 'TLS 1.3 everywhere probed, and no expired or near-expiry certificate.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ab180/refs/heads/main/security/ab180-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Attribution
- Mobile Measurement
- Marketing
- Analytics
- Advertising
- Deep Linking
- Mobile
- Reporting
- South Korea
---
