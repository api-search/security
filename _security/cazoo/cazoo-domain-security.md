---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cazoo.co.uk
  spf: true
hosts:
- cert_expires: Sep 20 21:28:30 2026 GMT
  host: www.cazoo.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cazoo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cazoo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cazoo
provider_slug: cazoo
slug: cazoo-domain-security
source_filename: cazoo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cazoo.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 21:28:30 2026 GMT\n  hsts: null\ndomains:\n- domain: cazoo.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cazoo/refs/heads/main/security/cazoo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ecommerce
- Automotive
- Used Cars
- Retail
- Marketplace
- Consumer Finance
- United Kingdom
---
