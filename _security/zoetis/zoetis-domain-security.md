---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zoetis.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: zoetisdiagnostics.com
  spf: false
hosts:
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: www.zoetis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: www.zoetisdiagnostics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zoetis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zoetis, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zoetis
provider_slug: zoetis
slug: zoetis-domain-security
source_filename: zoetis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zoetis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.zoetisdiagnostics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zoetis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: zoetisdiagnostics.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoetis/refs/heads/main/security/zoetis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Animal Health
- Veterinary
- Diagnostics
- Life Sciences
---
