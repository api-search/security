---
api_specs:
- filename: adbtd-com-openapi-generated.yml
  format: yaml
  label: adbtd API
  slug: adbtd-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adbtd-com/openapi/_ae-authored/adbtd-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adbtd.com
  spf: true
hosts:
- cert_expires: Jan 14 13:32:28 2027 GMT
  host: adbtd.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adbtd Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for adbtd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: adbtd
provider_slug: adbtd-com
slug: adbtd-com-domain-security
source_filename: adbtd-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adbtd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 13:32:28 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: adbtd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/adbtd-com/security/adbtd-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Infrastructure
- SMTP
- IMAP
- Dedicated IP
- Deliverability
- Webhook
- MCP
---
