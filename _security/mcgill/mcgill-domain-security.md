---
api_specs:
- filename: mcgill-dataverses-api-openapi.yml
  format: yaml
  label: McGill University Dataverses API
  slug: mcgill-dataverses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcgill/refs/heads/main/openapi/mcgill-dataverses-api-openapi.yml
- filename: mcgill-info-api-openapi.yml
  format: yaml
  label: McGill University Info API
  slug: mcgill-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcgill/refs/heads/main/openapi/mcgill-info-api-openapi.yml
- filename: mcgill-search-api-openapi.yml
  format: yaml
  label: McGill University Search API
  slug: mcgill-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcgill/refs/heads/main/openapi/mcgill-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mcgill.ca
  spf: true
- caa:
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: borealisdata.ca
  spf: true
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.mcgill.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: borealisdata.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 30 23:59:59 2026 GMT
  host: guides.dataverse.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mcgill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for McGill University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: McGill University
provider_slug: mcgill
slug: mcgill-domain-security
source_filename: mcgill-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mcgill.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: borealisdata.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: guides.dataverse.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: mcgill.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: borealisdata.ca\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mcgill/refs/heads/main/security/mcgill-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research Data
- Open Data
- Canada
- Quebec
---
