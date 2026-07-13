---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: corkcity.ie
  spf: true
hosts:
- cert_expires: Aug 26 23:46:38 2026 GMT
  host: data.corkcity.ie
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Data Corkcity Ie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cork City Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cork City Open Data
provider_slug: data-corkcity-ie
slug: data-corkcity-ie-domain-security
source_filename: data-corkcity-ie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.corkcity.ie\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 23:46:38 2026 GMT\n  hsts: false\ndomains:\n- domain: corkcity.ie\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-corkcity-ie/refs/heads/main/security/data-corkcity-ie-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Municipal Government
- Ireland
---
