---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: luxcreo.com
  spf: true
hosts:
- cert_expires: Sep 28 08:11:58 2026 GMT
  host: www.luxcreo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Luxcreo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LuxCreo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LuxCreo
provider_slug: luxcreo
slug: luxcreo-domain-security
source_filename: luxcreo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.luxcreo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 08:11:58 2026 GMT\n  hsts: false\ndomains:\n- domain: luxcreo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luxcreo/refs/heads/main/security/luxcreo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Hardtech
- 3D Printing
- Additive Manufacturing
- Dental
- Digital Dentistry
- Clear Aligners
- Manufacturing
---
