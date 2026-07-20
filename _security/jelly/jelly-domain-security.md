---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getjelly.co.uk
  spf: true
hosts:
- cert_expires: Sep 15 06:42:28 2026 GMT
  host: www.getjelly.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: docs.getjelly.co.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: api.getjelly.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jelly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jelly, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jelly
provider_slug: jelly
slug: jelly-domain-security
source_filename: jelly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getjelly.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 06:42:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.getjelly.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: false\n- host: api.getjelly.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: getjelly.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jelly/refs/heads/main/security/jelly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hospitality
- Restaurants
- Kitchen Management
- Food Costing
- Recipe Costing
- Invoice Processing
- GraphQL
- SaaS
---
