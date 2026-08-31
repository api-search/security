---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: unilever.com
  spf: true
hosts:
- cert_expires: Sep 21 02:51:49 2026 GMT
  host: www.unilever.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unilever Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unilever, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Unilever
provider_slug: unilever
slug: unilever-domain-security
source_filename: unilever-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unilever.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 02:51:49 2026 GMT\n  hsts: null\ndomains:\n- domain: unilever.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unilever/refs/heads/main/security/unilever-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Consumer Products
- Personal Care
- Food & Beverage
- Household Products
---
