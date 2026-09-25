---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nielsen.com
  spf: true
hosts:
- cert_expires: Nov 14 18:18:08 2026 GMT
  host: nielsen.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nielsen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nielsen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nielsen
provider_slug: nielsen
slug: nielsen-domain-security
source_filename: nielsen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nielsen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 18:18:08 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: nielsen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nielsen/refs/heads/main/security/nielsen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Audience Measurement
- Media Analytics
- DataInsights
- Marketing
---
