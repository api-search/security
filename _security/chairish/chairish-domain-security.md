---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chairish.com
  spf: true
hosts:
- cert_expires: Nov 15 22:03:26 2026 GMT
  host: www.chairish.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chairish Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chairish, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Chairish
provider_slug: chairish
slug: chairish-domain-security
source_filename: chairish-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chairish.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 15 22:03:26 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: chairish.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chairish/refs/heads/main/security/chairish-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Marketplace
- Vintage
- Furniture
- E-commerce
- Art
---
