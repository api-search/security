---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: yourcounterpart.com
  spf: true
hosts:
- cert_expires: Oct 19 05:53:11 2026 GMT
  host: yourcounterpart.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yourcounterpart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yourcounterpart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Yourcounterpart
provider_slug: yourcounterpart
slug: yourcounterpart-domain-security
source_filename: yourcounterpart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yourcounterpart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 05:53:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: yourcounterpart.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yourcounterpart/refs/heads/main/security/yourcounterpart-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Insurtech
- Management Liability
- Professional Liability
- Underwriting
- Quote and Bind
- Small Business
- API Partner
- Brokers
- Financial Services
---
