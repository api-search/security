---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: allianz.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: allianz-trade.com
  spf: true
hosts:
- cert_expires: Aug 12 16:58:20 2026 GMT
  host: www.allianz.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 05:28:28 2026 GMT
  host: developers.allianz-trade.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 23:51:50 2026 GMT
  host: globaldigitalfactory.allianz.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Allianz Technology Standards Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Allianz Technology Standards, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Allianz Technology Standards
provider_slug: allianz-technology-standards
slug: allianz-technology-standards-domain-security
source_filename: allianz-technology-standards-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.allianz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 16:58:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.allianz-trade.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 05:28:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: globaldigitalfactory.allianz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:51:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: allianz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: allianz-trade.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allianz-technology-standards/refs/heads/main/security/allianz-technology-standards-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Best Practices
- Enterprise Architecture
- Guidelines
- Software Development
- Technology Standards
- API Design
- OpenAPI
---
