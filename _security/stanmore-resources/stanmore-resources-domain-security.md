---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stanmore.au
  spf: true
hosts:
- cert_expires: Apr  3 23:59:59 2027 GMT
  host: stanmore.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Stanmore Resources Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stanmore Resources, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Stanmore Resources
provider_slug: stanmore-resources
slug: stanmore-resources-domain-security
source_filename: stanmore-resources-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stanmore.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stanmore.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stanmore-resources/refs/heads/main/security/stanmore-resources-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mining
- Metallurgical Coal
- Australia
- Natural Resources
- ASX Listed
---
