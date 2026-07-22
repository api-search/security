---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: selency.fr
  spf: true
hosts:
- cert_expires: Nov  3 23:59:59 2026 GMT
  host: www.selency.fr
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Selency Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Selency, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Selency
provider_slug: selency
slug: selency-domain-security
source_filename: selency-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.selency.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: selency.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/selency/refs/heads/main/security/selency-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Marketplace
- Furniture
- Home Decor
- Second-hand
- Vintage
- E-commerce
- France
---
