---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "starfieldtech.com"
  - 0 iodef "mailto:domainadmin@blackline.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blackline.com
  spf: true
hosts:
- cert_expires: Sep 12 05:34:30 2026 GMT
  host: www.blackline.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blackline Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlackLine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BlackLine
provider_slug: blackline
slug: blackline-domain-security
source_filename: blackline-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blackline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 05:34:30 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: blackline.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"starfieldtech.com\"\n  - 0 iodef \"mailto:domainadmin@blackline.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blackline/refs/heads/main/security/blackline-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- FinOps
- Accounting
- Financial Close
- Reconciliation
- Accounting Automation
- ERP Integration
- Enterprise Software
---
