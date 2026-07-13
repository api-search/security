---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: datamillnorth.org
  spf: false
hosts:
- cert_expires: Sep 10 10:07:09 2026 GMT
  host: datamillnorth.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datamillnorth Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Data Mill North (Leeds), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Data Mill North (Leeds)
provider_slug: datamillnorth-org
slug: datamillnorth-org-domain-security
source_filename: datamillnorth-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datamillnorth.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 10:07:09 2026 GMT\n  hsts: null\ndomains:\n- domain: datamillnorth.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datamillnorth-org/refs/heads/main/security/datamillnorth-org-domain-security.yml
summary_line: TLSv1.3
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Local Council
- United Kingdom
---
