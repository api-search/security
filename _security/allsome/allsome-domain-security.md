---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: allsome.my
  spf: true
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: allsome.my
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Allsome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AllSome, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AllSome
provider_slug: allsome
slug: allsome-domain-security
source_filename: allsome-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: allsome.my\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: allsome.my\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allsome/refs/heads/main/security/allsome-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- E-commerce
- Fulfillment
- Logistics
- Warehousing
- Cross-border
- Supply Chain
- Southeast Asia
---
