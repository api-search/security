---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cro.ie
  spf: true
hosts:
- cert_expires: Sep 21 06:30:52 2026 GMT
  host: opendata.cro.ie
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opendata Cro Ie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Companies Registration Office Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Companies Registration Office Open Data
provider_slug: opendata-cro-ie
slug: opendata-cro-ie-domain-security
source_filename: opendata-cro-ie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opendata.cro.ie\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 06:30:52 2026 GMT\n  hsts: false\ndomains:\n- domain: cro.ie\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opendata-cro-ie/refs/heads/main/security/opendata-cro-ie-domain-security.yml
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
