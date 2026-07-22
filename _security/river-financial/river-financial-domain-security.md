---
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@river.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: river.com
  spf: true
hosts:
- cert_expires: Sep  2 10:05:56 2026 GMT
  host: river.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: River Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for River Financial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: River Financial
provider_slug: river-financial
slug: river-financial-domain-security
source_filename: river-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: river.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 10:05:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: river.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:security@river.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/river-financial/refs/heads/main/security/river-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Bitcoin Services
- Cryptocurrency
- Financial Services
- Banking
- OAuth
- API
---
