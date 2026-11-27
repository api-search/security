---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: tendeta.io
  spf: true
hosts:
- cert_expires: Dec 27 21:43:26 2026 GMT
  host: tendeta.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tendeta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tendeta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tendeta
provider_slug: tendeta-io
slug: tendeta-io-domain-security
source_filename: tendeta-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tendeta.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 21:43:26 2026 GMT\n  hsts: false\ndomains:\n- domain: tendeta.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tendeta-io/security/tendeta-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- e-commerce
- no-code
- storefront
- micro-entrepreneur
- SaaS
---
