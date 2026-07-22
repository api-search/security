---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: starburstdata.com
  spf: true
hosts:
- cert_expires: Oct  1 06:16:40 2026 GMT
  host: starburstdata.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Starburst Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Starburst, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Starburst
provider_slug: starburst
slug: starburst-domain-security
source_filename: starburst-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: starburstdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 06:16:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: starburstdata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/starburst/refs/heads/main/security/starburst-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Analytics
- Data Lakehouse
- SQL Query Engine
- Trino
- Federated Query
- Data Governance
- Business Intelligence
---
