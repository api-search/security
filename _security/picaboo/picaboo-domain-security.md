---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: picaboo.com
  spf: true
hosts:
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: www.picaboo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Picaboo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Picaboo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Picaboo
provider_slug: picaboo
slug: picaboo-domain-security
source_filename: picaboo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.picaboo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: picaboo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/picaboo/security/picaboo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Photo
- Printing
- E-commerce
- SaaS
---
