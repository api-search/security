---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: osmos.io
  spf: true
hosts:
- cert_expires: Sep 13 17:13:46 2026 GMT
  host: osmos.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Osmos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Osmos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Osmos
provider_slug: osmos
slug: osmos-domain-security
source_filename: osmos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: osmos.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 17:13:46 2026 GMT\n  hsts: null\ndomains:\n- domain: osmos.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/osmos/refs/heads/main/security/osmos-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Data Ingestion
- Data Onboarding
- Data Integration
- ETL
- Data Import
- Artificial Intelligence
- Data Pipelines
- Data Quality
---
