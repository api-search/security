---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: koloma.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: kolomacalifornia.com
  spf: true
hosts:
- cert_expires: Oct  5 18:52:49 2026 GMT
  host: www.koloma.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 18:16:45 2026 GMT
  host: www.kolomacalifornia.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Koloma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Koloma, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Koloma
provider_slug: koloma
slug: koloma-domain-security
source_filename: koloma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.koloma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 18:52:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.kolomacalifornia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 18:16:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: koloma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: kolomacalifornia.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koloma/refs/heads/main/security/koloma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Energy
- Clean Energy
- Hydrogen
- Natural Hydrogen
- Geologic Hydrogen
- Exploration
- Geoscience
- Climate Tech
- Decarbonization
---
