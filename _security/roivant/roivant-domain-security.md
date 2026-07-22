---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: roivant.com
  spf: true
hosts:
- cert_expires: Aug 20 21:32:37 2026 GMT
  host: roivant.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Roivant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Roivant, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Roivant
provider_slug: roivant
slug: roivant-domain-security
source_filename: roivant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: roivant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 21:32:37 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: roivant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roivant/refs/heads/main/security/roivant-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health Tech
- Biopharmaceutical
- Pharmaceuticals
- Drug Development
- Life Sciences
- Immunology
---
