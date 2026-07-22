---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lotame.com
  spf: true
hosts:
- cert_expires: Oct  9 04:12:10 2026 GMT
  host: www.lotame.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 10:18:42 2026 GMT
  host: my.lotame.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: api.lotame.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lotame Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lotame Solutions, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lotame Solutions
provider_slug: lotame-solutions
slug: lotame-solutions-domain-security
source_filename: lotame-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lotame.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 04:12:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: my.lotame.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 10:18:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lotame.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: lotame.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lotame-solutions/refs/heads/main/security/lotame-solutions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Management Platform
- Identity
- Advertising
- Marketing
- Audience Data
- Data Collaboration
- AdTech
---
