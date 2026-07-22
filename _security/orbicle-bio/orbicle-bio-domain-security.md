---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: orbiclebio.com
  spf: false
hosts:
- cert_expires: Oct 13 23:26:52 2026 GMT
  host: orbiclebio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orbicle Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orbicle Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Orbicle Bio
provider_slug: orbicle-bio
slug: orbicle-bio-domain-security
source_filename: orbicle-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orbiclebio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:26:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: orbiclebio.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orbicle-bio/refs/heads/main/security/orbicle-bio-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biotechnology
- Agriculture
- Climate Tech
- Fertilizers
- Sustainability
---
