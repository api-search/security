---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: southerncompanygas.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: atlantagaslight.com
  spf: false
hosts:
- cert_expires: Aug 16 00:52:46 2026 GMT
  host: southerncompanygas.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 00:52:46 2026 GMT
  host: www.atlantagaslight.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agl Resources Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for agl-resources, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: agl-resources
provider_slug: agl-resources
slug: agl-resources-domain-security
source_filename: agl-resources-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: southerncompanygas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 00:52:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.atlantagaslight.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 00:52:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: southerncompanygas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: atlantagaslight.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agl-resources/refs/heads/main/security/agl-resources-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Natural Gas
- Utilities
- Energy Distribution
- Georgia
- Fortune 500
---
