---
api_specs:
- filename: altinity-acm-openapi-original.json
  format: json
  label: Altinity Cloud Manager API
  slug: altinity-cloud-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altinity/refs/heads/main/openapi/altinity-acm-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: altinity.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: altinity.cloud
  spf: true
hosts:
- cert_expires: Sep 26 04:12:58 2026 GMT
  host: altinity.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: acm.altinity.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Altinity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Altinity, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Altinity
provider_slug: altinity
slug: altinity-domain-security
source_filename: altinity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: altinity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 04:12:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: acm.altinity.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: altinity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: altinity.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/altinity/refs/heads/main/security/altinity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Big Data
- ClickHouse
- Analytics
- Database
- Managed Cloud
- Kubernetes
- Real-Time Analytics
- Open Source
---
