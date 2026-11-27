---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: parcelsheet.org
  spf: true
hosts:
- cert_expires: Jan 10 06:36:33 2027 GMT
  host: parcelsheet.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ParcelSheet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ParcelSheet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: ParcelSheet
provider_slug: parcelsheet-org
slug: parcelsheet-org-domain-security
source_filename: parcelsheet-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parcelsheet.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 06:36:33 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: parcelsheet.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/parcelsheet-org/security/parcelsheet-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Real Estate
- GIS
- Mapping
- Public Records
- Parcel Data
---
