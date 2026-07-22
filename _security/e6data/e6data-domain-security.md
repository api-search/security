---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: e6data.com
  spf: true
hosts:
- cert_expires: Sep 29 06:43:21 2026 GMT
  host: www.e6data.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: E6Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for e6data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: e6data
provider_slug: e6data
slug: e6data-domain-security
source_filename: e6data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.e6data.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 06:43:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: e6data.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/e6data/refs/heads/main/security/e6data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- B2B
- Data
- Analytics
- Lakehouse
- SQL
- Query Engine
- Data Infrastructure
- Big Data
---
