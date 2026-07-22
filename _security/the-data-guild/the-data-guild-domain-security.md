---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: thedataguild.com
  spf: false
hosts:
- cert_expires: Oct 13 18:03:46 2026 GMT
  host: www.thedataguild.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Data Guild Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Data Guild, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: The Data Guild
provider_slug: the-data-guild
slug: the-data-guild-domain-security
source_filename: the-data-guild-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thedataguild.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 18:03:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: thedataguild.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-data-guild/refs/heads/main/security/the-data-guild-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Venture Studio
- Data Science
- Machine Learning
- Artificial Intelligence
- Healthcare
- Climate
---
