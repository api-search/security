---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: forhims.com
  spf: true
hosts:
- cert_expires: Oct  8 18:17:54 2026 GMT
  host: forhims.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hims Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hims, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hims
provider_slug: hims
slug: hims-domain-security
source_filename: hims-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forhims.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  8 18:17:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: forhims.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hims/refs/heads/main/security/hims-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Telehealth
- Wellness
- Pharmacy
- Consumer
- E-commerce
---
