---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tryalma.com
  spf: true
hosts:
- cert_expires: Aug 24 06:18:11 2026 GMT
  host: www.tryalma.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Alma
provider_slug: alma
slug: alma-domain-security
source_filename: alma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tryalma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 06:18:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tryalma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alma/refs/heads/main/security/alma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Immigration
- Legal
- LegalTech
- Visas
- Global Mobility
- Compliance
- Immigration Software
---
