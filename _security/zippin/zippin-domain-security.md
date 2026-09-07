---
description: ''
domains:
- caa:
  - 0 issue "www.digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@getzippin.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getzippin.com
  spf: true
hosts:
- cert_expires: Oct 12 23:44:39 2026 GMT
  host: www.getzippin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 23:03:28 2026 GMT
  host: api.getzippin.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Zippin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zippin, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zippin
provider_slug: zippin
slug: zippin-domain-security
source_filename: zippin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getzippin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:44:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getzippin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 23:03:28 2026 GMT\n  hsts: null\ndomains:\n- domain: getzippin.com\n  dnssec: false\n  caa:\n  - 0 issue \"www.digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@getzippin.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zippin/refs/heads/main/security/zippin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- Retail Technology
- Checkout Free
- Cashierless
- Computer Vision
- Artificial Intelligence
- Machine Learning
- Point of Sale
- Payments
- Loyalty
- Inventory
- Sports Venues
- Airports
- Higher Education
---
