---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: arbol.io
  spf: true
hosts:
- cert_expires: Nov 29 13:33:46 2026 GMT
  host: www.arbol.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arbolmarkets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arbolmarkets, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Arbolmarkets
provider_slug: arbolmarkets
slug: arbolmarkets-domain-security
source_filename: arbolmarkets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arbol.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 13:33:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: arbol.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arbolmarkets/refs/heads/main/security/arbolmarkets-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
---
