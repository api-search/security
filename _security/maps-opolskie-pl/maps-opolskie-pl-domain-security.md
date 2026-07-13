---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: opolskie.pl
  spf: true
hosts:
- cert_expires: Dec  5 07:58:53 2026 GMT
  host: maps.opolskie.pl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Maps Opolskie Pl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opolskie Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Opolskie Open Data
provider_slug: maps-opolskie-pl
slug: maps-opolskie-pl-domain-security
source_filename: maps-opolskie-pl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maps.opolskie.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 07:58:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opolskie.pl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maps-opolskie-pl/refs/heads/main/security/maps-opolskie-pl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Data
- DKAN
- Data Catalog
- DCAT
- Government Data
- Regional Government
- Poland
---
