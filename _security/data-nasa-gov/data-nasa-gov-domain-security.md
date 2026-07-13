---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nasa.gov
  spf: true
hosts:
- cert_expires: Sep  3 11:13:07 2026 GMT
  host: data.nasa.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Data Nasa Gov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NASA Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: NASA Open Data
provider_slug: data-nasa-gov
slug: data-nasa-gov-domain-security
source_filename: data-nasa-gov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.nasa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 11:13:07 2026 GMT\n  hsts: null\ndomains:\n- domain: nasa.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-nasa-gov/refs/heads/main/security/data-nasa-gov-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Federal Government
- United States
---
