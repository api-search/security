---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: amerisourcebergen.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cencora.com
  spf: true
hosts:
- cert_expires: Sep  1 23:59:59 2026 GMT
  host: www.amerisourcebergen.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: www.cencora.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Amerisourcebergen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AmerisourceBergen, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AmerisourceBergen
provider_slug: amerisourcebergen
slug: amerisourcebergen-domain-security
source_filename: amerisourcebergen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amerisourcebergen.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.cencora.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: amerisourcebergen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cencora.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amerisourcebergen/refs/heads/main/security/amerisourcebergen-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Pharmaceutical Distribution
- Healthcare
- Drug Distribution
- Manufacturer Solutions
- Provider Solutions
- Animal Health
- Life Sciences
- Fortune 100
---
