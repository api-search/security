---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: howdengroup.com
  spf: true
hosts:
- cert_expires: Sep  7 14:25:37 2026 GMT
  host: www.howdengroup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: parentportal.howdengroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Howden Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Howden Group, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Howden Group
provider_slug: howden-group
slug: howden-group-domain-security
source_filename: howden-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.howdengroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 14:25:37 2026 GMT\n  hsts: false\n- host: parentportal.howdengroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: howdengroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/howden-group/refs/heads/main/security/howden-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- United Kingdom
- Broker
- Insurance Broking
- Reinsurance
- Specialty Insurance
- Managing General Agent
- Employee Benefits
- Credit Insurance
- London Market
- ACORD
- Partner Gated
---
