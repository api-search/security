---
description: ''
domains:
- caa:
  - 0 issue "Digicert.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: addepar.com
  spf: true
hosts:
- cert_expires: Sep 30 06:03:46 2026 GMT
  host: addepar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Addepar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Addepar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Addepar
provider_slug: addepar
slug: addepar-domain-security
source_filename: addepar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: addepar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 06:03:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: addepar.com\n  dnssec: false\n  caa:\n  - 0 issue \"Digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/addepar/refs/heads/main/security/addepar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Wealth Management
- Portfolio Management
- Investment Management
- Financial Data
- JSON:API
- REST
---
