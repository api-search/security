---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: madeincookware.com
  spf: true
hosts:
- cert_expires: Nov 29 21:39:12 2026 GMT
  host: madeincookware.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Made In Cookware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Made In Cookware, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Made In Cookware
provider_slug: made-in-cookware
slug: made-in-cookware-domain-security
source_filename: made-in-cookware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: madeincookware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 21:39:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: madeincookware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/made-in-cookware/refs/heads/main/security/made-in-cookware-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cookware
- E-Commerce
- Direct to Consumer
- Kitchenware
- Premium
---
