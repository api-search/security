---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: boston.gov
  spf: true
hosts:
- cert_expires: Oct  4 18:22:41 2026 GMT
  host: data.boston.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Data Boston Gov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Analyze Boston, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Analyze Boston
provider_slug: data-boston-gov
slug: data-boston-gov-domain-security
source_filename: data-boston-gov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.boston.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 18:22:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: boston.gov\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-boston-gov/refs/heads/main/security/data-boston-gov-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Municipal Government
- United States
---
