---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: elementl.com
  spf: true
hosts:
- cert_expires: Dec 27 01:13:34 2026 GMT
  host: elementl.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elementl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elementl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Elementl
provider_slug: elementl
slug: elementl-domain-security
source_filename: elementl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elementl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 01:13:34 2026 GMT\n  hsts: null\ndomains:\n- domain: elementl.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elementl/refs/heads/main/security/elementl-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Open Source
- Data Orchestration
- Data Engineering
- Data Pipelines
- DataOps
- Observability
- Analytics
- Machine Learning
- Cloud
---
