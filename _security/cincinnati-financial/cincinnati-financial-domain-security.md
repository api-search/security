---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cinfin.com
  spf: true
hosts:
- cert_expires: Aug  7 23:59:59 2026 GMT
  host: www.cinfin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cincinnati Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cincinnati Financial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cincinnati Financial
provider_slug: cincinnati-financial
slug: cincinnati-financial-domain-security
source_filename: cincinnati-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cinfin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cinfin.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cincinnati-financial/refs/heads/main/security/cincinnati-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Auto Insurance
- Business Insurance
- Financial Services
- Home Insurance
- Independent Agency
- Insurance
- Life Insurance
- No Public API
- Property Casualty
- Fortune 1000
---
