---
api_specs:
- filename: channel99-pulsar-openapi.json
  format: json
  label: Channel99 Pulsar Reporting API
  slug: channel99-pulsar-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channel99/refs/heads/main/openapi/channel99-pulsar-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: channel99.com
  spf: true
hosts:
- cert_expires: Oct  2 01:27:01 2026 GMT
  host: channel99.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:49:36 2026 GMT
  host: support.channel99.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: pulsar.channel99.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Channel99 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Channel99, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Channel99
provider_slug: channel99
slug: channel99-domain-security
source_filename: channel99-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: channel99.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 01:27:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.channel99.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:49:36 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: pulsar.channel99.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: channel99.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/channel99/refs/heads/main/security/channel99-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketing
- Analytics
- Attribution
- B2B
- Advertising
- Marketing Technology
- Artificial Intelligence
- Account Based Marketing
- Reporting
- MCP
- Agent Ready
- Intent Data
- Account Identification
- Data Export
---
