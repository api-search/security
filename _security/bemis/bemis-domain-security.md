---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amcor.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: bemisus.com
  spf: false
hosts:
- cert_expires: Sep 11 09:03:56 2026 GMT
  host: www.amcor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 13:06:39 2026 GMT
  host: www.bemisus.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bemis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bemis, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bemis
provider_slug: bemis
slug: bemis-domain-security
source_filename: bemis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amcor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 09:03:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.bemisus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 13:06:39 2026 GMT\n  hsts: null\ndomains:\n- domain: amcor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: bemisus.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bemis/refs/heads/main/security/bemis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amcor
- Consumer Packaging
- Flexible Packaging
- Food Packaging
- Healthcare Packaging
- Manufacturing
- Packaging
- Pharmaceutical Packaging
---
