---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: podatki.gov.si
  spf: false
hosts:
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: podatki.gov.si
  hsts: true
  hsts_max_age: 48000000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Podatki Gov Si Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OPSI Slovenia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OPSI Slovenia
provider_slug: podatki-gov-si
slug: podatki-gov-si-domain-security
source_filename: podatki-gov-si-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: podatki.gov.si\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 48000000\ndomains:\n- domain: podatki.gov.si\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/podatki-gov-si/refs/heads/main/security/podatki-gov-si-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- National Government
- Slovenia
---
