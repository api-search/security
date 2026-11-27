---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cdc.gov
  spf: true
hosts:
- cert_expires: May  5 23:59:59 2027 GMT
  host: www.cdc.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NHANES (CDC) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NHANES (CDC), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: NHANES (CDC)
provider_slug: nhanes
slug: nhanes-domain-security
source_filename: nhanes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cdc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: cdc.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/nhanes/security/nhanes-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Public Health
- Health Statistics
- Nutrition
- Open Data
- Survey Data
- Government
- CDC
---
