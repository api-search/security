---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: billiontoone.com
  spf: true
hosts:
- cert_expires: Sep 23 19:49:57 2026 GMT
  host: billiontoone.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Billiontoone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BillionToOne, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BillionToOne
provider_slug: billiontoone
slug: billiontoone-domain-security
source_filename: billiontoone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: billiontoone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 19:49:57 2026 GMT\n  hsts: false\ndomains:\n- domain: billiontoone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/billiontoone/refs/heads/main/security/billiontoone-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Molecular Diagnostics
- Healthcare
- Genomics
- Prenatal Testing
- Oncology
- Liquid Biopsy
- Diagnostics
---
