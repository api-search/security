---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: totusmedicines.com
  spf: true
hosts:
- cert_expires: Sep 26 17:29:46 2026 GMT
  host: www.totusmedicines.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Totus Medicines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Totus Medicines, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Totus Medicines
provider_slug: totus-medicines
slug: totus-medicines-domain-security
source_filename: totus-medicines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.totusmedicines.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 17:29:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: totusmedicines.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/totus-medicines/refs/heads/main/security/totus-medicines-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biopharmaceutical
- Drug Discovery
- Covalent Small Molecules
- Oncology
- Immunology
- Precision Medicine
- Biotechnology
---
