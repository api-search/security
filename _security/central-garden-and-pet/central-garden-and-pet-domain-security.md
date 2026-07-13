---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: central.com
  spf: true
hosts:
- cert_expires: Sep  7 02:59:27 2026 GMT
  host: www.central.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.central.com
  https: false
- cert_expires: Oct 30 16:37:41 2026 GMT
  host: api.central.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Central Garden And Pet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Central Garden and Pet, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Central Garden and Pet
provider_slug: central-garden-and-pet
slug: central-garden-and-pet-domain-security
source_filename: central-garden-and-pet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.central.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 02:59:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.central.com\n  https: false\n- host: api.central.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 30 16:37:41 2026 GMT\n  hsts: false\ndomains:\n- domain: central.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/central-garden-and-pet/refs/heads/main/security/central-garden-and-pet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Pet Products
- Garden
- Consumer
---
