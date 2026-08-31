---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ca.gov
  spf: true
hosts:
- cert_expires: Oct  4 11:08:47 2026 GMT
  host: data.cnra.ca.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Data Cnra Ca Gov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for California Natural Resources Agency, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: California Natural Resources Agency
provider_slug: data-cnra-ca-gov
slug: data-cnra-ca-gov-domain-security
source_filename: data-cnra-ca-gov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.cnra.ca.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 11:08:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ca.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-cnra-ca-gov/refs/heads/main/security/data-cnra-ca-gov-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- State Government
- United States
---
