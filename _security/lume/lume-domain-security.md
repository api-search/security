---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lume.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: lume-terminus.com
  spf: false
hosts:
- cert_expires: Oct  5 00:44:37 2026 GMT
  host: docs.lume.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: prod.lume-terminus.com
  https: false
kind: domain-security
layout: security
method: probed
name: Lume Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lume, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lume
provider_slug: lume
slug: lume-domain-security
source_filename: lume-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.lume.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 00:44:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: prod.lume-terminus.com\n  https: false\ndomains:\n- domain: lume.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: lume-terminus.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lume/refs/heads/main/security/lume-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Integration
- Data Mapping
- ETL
- Data Transformation
- Artificial Intelligence
- Schema Mapping
- Data Quality
- Developer Tools
---
