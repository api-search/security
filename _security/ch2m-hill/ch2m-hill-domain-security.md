---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jacobs.com
  spf: true
hosts:
- cert_expires: Aug 17 23:38:24 2026 GMT
  host: www.jacobs.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ch2M Hill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CH2M Hill, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CH2M Hill
provider_slug: ch2m-hill
slug: ch2m-hill-domain-security
source_filename: ch2m-hill-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jacobs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 23:38:24 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: jacobs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ch2m-hill/refs/heads/main/security/ch2m-hill-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Acquired
- Construction
- Consulting
- Engineering
- Government
- Infrastructure
---
