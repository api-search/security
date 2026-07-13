---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bc.ca
  spf: false
hosts:
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: www.data.gov.bc.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Data Gov Bc Ca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for British Columbia (DataBC), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: British Columbia (DataBC)
provider_slug: data-gov-bc-ca
slug: data-gov-bc-ca-domain-security
source_filename: data-gov-bc-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.data.gov.bc.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: bc.ca\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-gov-bc-ca/refs/heads/main/security/data-gov-bc-ca-domain-security.yml
summary_line: TLSv1.3
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Open Data Portal
- Canada
---
