---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tiffany.com
  spf: true
hosts:
- cert_expires: Nov  3 23:59:59 2026 GMT
  host: www.tiffany.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tiffany Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tiffany & Co., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tiffany & Co.
provider_slug: tiffany
slug: tiffany-domain-security
source_filename: tiffany-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tiffany.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tiffany.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tiffany/refs/heads/main/security/tiffany-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Corporate Gifting
- E-Commerce
- Jewelry
- Luxury Retail
- Watches
- Fortune 1000
---
