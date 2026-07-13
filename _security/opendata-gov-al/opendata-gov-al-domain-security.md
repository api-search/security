---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: opendata.gov.al
  spf: true
hosts:
- cert_expires: Aug 15 23:59:59 2026 GMT
  host: opendata.gov.al
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Opendata Gov Al Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for opendata.gov.al (Open Data Albania), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: opendata.gov.al (Open Data Albania)
provider_slug: opendata-gov-al
slug: opendata-gov-al-domain-security
source_filename: opendata-gov-al-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opendata.gov.al\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 15 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: opendata.gov.al\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opendata-gov-al/refs/heads/main/security/opendata-gov-al-domain-security.yml
summary_line: TLSv1.2
tags:
- Open Data
- Custom Platform
- DCAT-AP
- SPARQL
- Linked Data
- Government Data
- National Government
- Albania
- Europe
---
