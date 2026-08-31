---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sqream.com
  spf: true
hosts:
- cert_expires: Oct 29 13:55:02 2026 GMT
  host: sqream.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sqream Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SQream Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SQream Technologies
provider_slug: sqream-technologies
slug: sqream-technologies-domain-security
source_filename: sqream-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sqream.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 13:55:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sqream.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sqream-technologies/refs/heads/main/security/sqream-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Database
- Data Warehouse
- Analytics
- GPU
- SQL
- Big Data
- Machine-Learning
- Data Ingestion
- Israel
---
