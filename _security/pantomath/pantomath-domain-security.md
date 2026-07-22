---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pantomath.com
  spf: true
hosts:
- cert_expires: Oct 14 18:00:00 2026 GMT
  host: www.pantomath.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pantomath Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pantomath, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pantomath
provider_slug: pantomath
slug: pantomath-domain-security
source_filename: pantomath-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pantomath.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 18:00:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pantomath.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pantomath/refs/heads/main/security/pantomath-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Observability
- Data Operations
- Data Pipeline Monitoring
- Data Lineage
- Data Quality
- Data Reliability
- Analytics
---
