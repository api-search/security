---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: makersite.io
  spf: true
hosts:
- cert_expires: Sep  9 23:32:45 2026 GMT
  host: makersite.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Makersite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Makersite, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Makersite
provider_slug: makersite
slug: makersite-domain-security
source_filename: makersite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: makersite.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:32:45 2026 GMT\n  hsts: false\ndomains:\n- domain: makersite.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/makersite/refs/heads/main/security/makersite-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Sustainability
- Product Lifecycle
- Supply Chain
- Compliance
- Carbon Footprint
- Life Cycle Assessment
- Manufacturing
---
