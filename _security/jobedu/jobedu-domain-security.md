---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jobedu.com
  spf: false
hosts:
- cert_expires: Aug 31 09:50:11 2026 GMT
  host: jobedu.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jobedu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jobedu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Jobedu
provider_slug: jobedu
slug: jobedu-domain-security
source_filename: jobedu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jobedu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 09:50:11 2026 GMT\n  hsts: null\ndomains:\n- domain: jobedu.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jobedu/refs/heads/main/security/jobedu-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Retail
- E-Commerce
- Shopify
- Consumer
- Merchandise
- Jordan
---
