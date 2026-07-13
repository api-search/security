---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: arkema.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bostik.com
  spf: true
hosts:
- cert_expires: Sep 30 05:43:54 2026 GMT
  host: www.arkema.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 11:50:26 2026 GMT
  host: www.bostik.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arkema Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arkema, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Arkema
provider_slug: arkema
slug: arkema-domain-security
source_filename: arkema-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arkema.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 05:43:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.bostik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 11:50:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: arkema.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: bostik.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arkema/refs/heads/main/security/arkema-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Chemicals
- Specialty Materials
- Adhesives
- Polymers
- Coatings
- Manufacturing
- Sustainability
---
