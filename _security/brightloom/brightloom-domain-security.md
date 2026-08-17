---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: brightloom.com
  spf: false
hosts:
- cert_expires: Sep 28 11:16:09 2026 GMT
  host: www.brightloom.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brightloom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brightloom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Brightloom
provider_slug: brightloom
slug: brightloom-domain-security
source_filename: brightloom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brightloom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 11:16:09 2026 GMT\n  hsts: false\ndomains:\n- domain: brightloom.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightloom/refs/heads/main/security/brightloom-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Customer Data Platform
- Customer Intelligence
- Restaurants
- Retail
- Marketing
- Loyalty
- Segmentation
- Point of Sale
- Analytics
---
