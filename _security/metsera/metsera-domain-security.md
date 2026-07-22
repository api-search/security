---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: metsera.com
  spf: true
hosts:
- cert_expires: Oct 12 10:03:39 2026 GMT
  host: metsera.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Metsera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metsera *, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Metsera *
provider_slug: metsera
slug: metsera-domain-security
source_filename: metsera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metsera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 10:03:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: metsera.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metsera/refs/heads/main/security/metsera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Life Sciences
- Biopharmaceutical
- Pharmaceuticals
- Obesity
- Metabolic Disease
- Drug Development
---
