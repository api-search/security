---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: carmoola.co.uk
  spf: true
hosts:
- cert_expires: Sep 29 06:28:31 2026 GMT
  host: www.carmoola.co.uk
  hsts: true
  hsts_max_age: 3628800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carmoola Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carmoola, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Carmoola
provider_slug: carmoola
slug: carmoola-domain-security
source_filename: carmoola-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carmoola.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 06:28:31 2026 GMT\n  hsts: true\n  hsts_max_age: 3628800\ndomains:\n- domain: carmoola.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carmoola/refs/heads/main/security/carmoola-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Automotive
- Car Finance
- Lending
- Consumer Credit
- United Kingdom
- Mobile App
---
