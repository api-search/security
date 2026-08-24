---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: isnetworld.com
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: www.isnetworld.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: api.isnetworld.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: HSTS was read from the Strict-Transport-Security header on the live HTTP 401 returned by GET https://api.isnetworld.com/token on 2026-08-23; the automated probe recorded null because the host answers no unauthenticated 200.
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Isn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ISN, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ISN
provider_slug: isn
slug: isn-domain-security
source_filename: isn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.isnetworld.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.isnetworld.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: >-\n    HSTS was read from the Strict-Transport-Security header on the live HTTP 401\n    returned by GET https://api.isnetworld.com/token on 2026-08-23; the automated\n    probe recorded null because the host answers no unauthenticated 200.\ndomains:\n- domain: isnetworld.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/isn/refs/heads/main/security/isn-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Contractor Management
- Supplier Management
- Health Safety and Environment
- Risk Management
- Compliance
- Supply Chain
- Sustainability
- Workforce
- Insurance
- Training
- Enterprise Software
---
