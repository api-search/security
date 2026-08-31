---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: juullabs.com
  spf: true
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: juul.com
  spf: true
hosts:
- cert_expires: Nov 14 18:25:20 2026 GMT
  host: www.juullabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: www.juul.com
  hsts: false
  https: true
  note: 'Consumer commerce host. Behind CloudFront + AWS WAF; non-static paths answer HTTP 202 with x-amzn-waf-action: challenge.'
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Juul Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JUUL, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: JUUL
provider_slug: juul
slug: juul-domain-security
source_filename: juul-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.juullabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 18:25:20 2026 GMT\n  hsts: false\n- host: www.juul.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: false\n  note: 'Consumer commerce host. Behind CloudFront + AWS WAF; non-static paths answer\n    HTTP 202 with x-amzn-waf-action: challenge.'\ndomains:\n- domain: juullabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: juul.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/juul/refs/heads/main/security/juul-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer Products
- Nicotine
- Vaping
- Hardware
- Consumer Electronics
- Bluetooth Low Energy
- Open-Source
- Kotlin Multiplatform
- Regulated Industry
---
