---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: teagasc.ie
  spf: true
hosts:
- cert_expires: Sep 17 03:38:25 2026 GMT
  host: opendata.teagasc.ie
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opendata Teagasc Ie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teagasc Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Teagasc Open Data
provider_slug: opendata-teagasc-ie
slug: opendata-teagasc-ie-domain-security
source_filename: opendata-teagasc-ie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opendata.teagasc.ie\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 03:38:25 2026 GMT\n  hsts: false\ndomains:\n- domain: teagasc.ie\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opendata-teagasc-ie/refs/heads/main/security/opendata-teagasc-ie-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Government Agency
- Ireland
---
