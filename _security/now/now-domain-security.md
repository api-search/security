---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "digicert.com"
  - 0 issue "amazonaws.com"
  - 0 issuemail "it-security@dnow.com"
  - 0 iodef "mailto:security@dnow.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dnow.com
  spf: true
hosts:
- cert_expires: Aug 15 20:45:56 2026 GMT
  host: www.dnow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: shop.dnow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Now Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DNOW, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DNOW
provider_slug: now
slug: now-domain-security
source_filename: now-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dnow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 20:45:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: shop.dnow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dnow.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issuemail \"it-security@dnow.com\"\n  - 0 iodef \"mailto:security@dnow.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/now/refs/heads/main/security/now-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Industrial Distribution
- Pipe Valves And Fittings
- PVF
- Supply Chain
- Procurement
- eCommerce
- cXML
- OCI
- Punchout
- IoT
- Inventory Management
- Mobile Apps
- Engineered Equipment
---
