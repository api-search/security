---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mitrachem.com
  spf: true
hosts:
- cert_expires: Sep 29 04:45:36 2026 GMT
  host: www.mitrachem.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mitra Chem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mitra Chem, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mitra Chem
provider_slug: mitra-chem
slug: mitra-chem-domain-security
source_filename: mitra-chem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mitrachem.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:45:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mitrachem.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mitra-chem/refs/heads/main/security/mitra-chem-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Battery Materials
- Advanced Manufacturing
- Energy Storage
- Chemicals
- Electric Vehicles
- Critical Minerals
- Artificial Intelligence
---
