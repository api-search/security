---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vendhq.com
  spf: true
hosts:
- cert_expires: Oct 10 10:32:33 2026 GMT
  host: www.vendhq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vend, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vend
provider_slug: vend
slug: vend-domain-security
source_filename: vend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vendhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 10:32:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: vendhq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vend/refs/heads/main/security/vend-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- Point of Sale
- Commerce
- Inventory
- Acquired
---
