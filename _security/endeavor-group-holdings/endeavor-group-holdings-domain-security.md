---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wmegrp.com
  spf: true
hosts:
- cert_expires: Sep 14 15:15:00 2026 GMT
  host: wmegrp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Endeavor Group Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Endeavor Group Holdings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Endeavor Group Holdings
provider_slug: endeavor-group-holdings
slug: endeavor-group-holdings-domain-security
source_filename: endeavor-group-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wmegrp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:15:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wmegrp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/endeavor-group-holdings/refs/heads/main/security/endeavor-group-holdings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sports
- Entertainment
- Talent
- Media
- Licensing
- Marketing
---
