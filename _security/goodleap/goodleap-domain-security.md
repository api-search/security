---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:security@goodleap.com"
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: goodleap.com
  spf: true
hosts:
- cert_expires: Oct 11 05:42:48 2026 GMT
  host: www.goodleap.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Goodleap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoodLeap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GoodLeap
provider_slug: goodleap
slug: goodleap-domain-security
source_filename: goodleap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.goodleap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 05:42:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: goodleap.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:security@goodleap.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goodleap/refs/heads/main/security/goodleap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Lending
- Financing
- Solar
- Home Improvement
- Point of Sale
- Sustainability
---
