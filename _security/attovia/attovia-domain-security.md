---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: attovia.com
  spf: true
hosts:
- cert_expires: Sep 24 13:01:21 2026 GMT
  host: www.attovia.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Attovia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Attovia Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Attovia Therapeutics
provider_slug: attovia
slug: attovia-domain-security
source_filename: attovia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.attovia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 13:01:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: attovia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attovia/refs/heads/main/security/attovia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Biopharmaceutical
- Life Sciences
- Immunology
- Therapeutics
- Drug Discovery
- Clinical Stage
---
