---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: manomano.co.uk
  spf: true
hosts:
- cert_expires: Sep 26 13:57:05 2026 GMT
  host: www.manomano.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Manomano Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ManoMano, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ManoMano
provider_slug: manomano
slug: manomano-domain-security
source_filename: manomano-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.manomano.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 13:57:05 2026 GMT\n  hsts: null\ndomains:\n- domain: manomano.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/manomano/refs/heads/main/security/manomano-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketplace
- DIY
- Home Improvement
- Gardening
- E-commerce
- Retail
- France
- Europe
---
