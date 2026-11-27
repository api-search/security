---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: geolithicintelligence.com
  spf: false
hosts:
- cert_expires: Feb  5 19:13:46 2027 GMT
  host: geolithicintelligence.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Atlas of Geolithic Intelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atlas of Geolithic Intelligence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Atlas of Geolithic Intelligence
provider_slug: geolithicintelligence-com
slug: geolithicintelligence-com-domain-security
source_filename: geolithicintelligence-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geolithicintelligence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 19:13:46 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: geolithicintelligence.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/geolithicintelligence-com/security/geolithicintelligence-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
