---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: southerncompany.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: southernco.com
  spf: true
hosts:
- cert_expires: Aug 16 00:52:46 2026 GMT
  host: www.southerncompany.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: customerservice2.southernco.com
  https: false
- cert_expires: Aug 16 00:52:46 2026 GMT
  host: investor.southerncompany.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Southern Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Southern Company, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Southern Company
provider_slug: southern
slug: southern-domain-security
source_filename: southern-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.southerncompany.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 00:52:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: customerservice2.southernco.com\n  https: false\n- host: investor.southerncompany.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 00:52:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: southerncompany.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: southernco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/southern/refs/heads/main/security/southern-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 500
- Electric Utility
- Natural Gas
- Energy
---
