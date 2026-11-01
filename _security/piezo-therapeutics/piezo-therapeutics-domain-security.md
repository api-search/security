---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: piezotx.com
  spf: true
hosts:
- cert_expires: Jan 17 17:12:45 2027 GMT
  host: piezotx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Piezo Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Piezo Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Piezo Therapeutics
provider_slug: piezo-therapeutics
slug: piezo-therapeutics-domain-security
source_filename: piezo-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: piezotx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 17:12:45 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: piezotx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/piezo-therapeutics/security/piezo-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Therapeutics
- Skin
- Regenerative
---
