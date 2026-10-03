---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bindolabs.com
  spf: true
hosts:
- cert_expires: Nov 28 00:39:33 2026 GMT
  host: bindolabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bindo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bindo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bindo
provider_slug: bindo
slug: bindo-domain-security
source_filename: bindo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bindolabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 00:39:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bindolabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bindo/refs/heads/main/security/bindo-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Point-of-Sale
- Retail
- Hospitality
- Payments
---
