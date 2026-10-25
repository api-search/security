---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: simsltd.com
  spf: true
hosts:
- cert_expires: Dec  5 23:53:07 2026 GMT
  host: simsltd.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sims Limited Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sims Limited, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sims Limited
provider_slug: sims-limited
slug: sims-limited-domain-security
source_filename: sims-limited-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: simsltd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:53:07 2026 GMT\n  hsts: false\ndomains:\n- domain: simsltd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sims-limited/refs/heads/main/security/sims-limited-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Recycling
- Metal Recycling
- Circular Economy
- Sustainability
- Australia
- ASX Listed
---
