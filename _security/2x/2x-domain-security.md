---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 2x.marketing
  spf: true
hosts:
- cert_expires: Oct  1 07:45:38 2026 GMT
  host: 2x.marketing
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 2X Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 2X, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 2X
provider_slug: 2x
slug: 2x-domain-security
source_filename: 2x-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 2x.marketing\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 07:45:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 2x.marketing\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/2x/refs/heads/main/security/2x-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketing
- Marketing as a Service
- B2B
- MarTech
- Marketing Operations
- Consulting
- Artificial Intelligence
---
