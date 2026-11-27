---
description: ''
domains:
- caa:
  - nkd-production-edbfbsbqg3gugnhs.a01.azurefd.net.
  - mr-a01.tm-azurefd.net.
  dmarc: false
  dnssec: true
  domain: data.gov.cz
  spf: false
hosts:
- cert_expires: Feb 28 23:59:59 2027 GMT
  host: data.gov.cz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Národní katalog otevřených dat (data.gov.cz) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Národní katalog otevřených dat (data.gov.cz), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Národní katalog otevřených dat (data.gov.cz)
provider_slug: open-government-czech-republic
slug: open-government-czech-republic-domain-security
source_filename: open-government-czech-republic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.gov.cz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: data.gov.cz\n  dnssec: true\n  caa:\n  - nkd-production-edbfbsbqg3gugnhs.a01.azurefd.net.\n  - mr-a01.tm-azurefd.net.\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/open-government-czech-republic/security/open-government-czech-republic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Government
- Open Data
- Czech Republic
- DCAT
- SPARQL
- GraphQL
- Linked Data
- Public APIs
---
