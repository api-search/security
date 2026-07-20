---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: happy.co
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: happyco.com
  spf: true
hosts:
- cert_expires: Oct  6 05:31:28 2026 GMT
  host: happy.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 00:02:54 2026 GMT
  host: developer.happy.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 07:09:43 2026 GMT
  host: grpc.happyco.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Happyco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HappyCo, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HappyCo
provider_slug: happyco
slug: happyco-domain-security
source_filename: happyco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: happy.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 05:31:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.happy.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 00:02:54 2026 GMT\n  hsts: false\n- host: grpc.happyco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 07:09:43 2026 GMT\n  hsts: null\ndomains:\n- domain: happy.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: happyco.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/happyco/refs/heads/main/security/happyco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- PropTech
- Real Estate
- Property Management
- Inspections
- Maintenance
- Multifamily
- gRPC
---
