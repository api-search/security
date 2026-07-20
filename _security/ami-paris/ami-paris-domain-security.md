---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: amiparis.com
  spf: true
hosts:
- cert_expires: Sep  3 16:01:35 2026 GMT
  host: amiparis.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ami Paris Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AMI Paris, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AMI Paris
provider_slug: ami-paris
slug: ami-paris-domain-security
source_filename: ami-paris-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amiparis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 16:01:35 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: amiparis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ami-paris/refs/heads/main/security/ami-paris-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Fashion
- Retail
- Ecommerce
- Shopify
- Agent Commerce
- UCP
---
