---
api_specs:
- filename: zenodo-rest-api-openapi.yml
  format: yaml
  label: Zenodo REST API
  slug: zenodo-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenodo/refs/heads/main/openapi/zenodo-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zenodo.org
  spf: true
hosts:
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: zenodo.org
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 13:57:49 2026 GMT
  host: developers.zenodo.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: sandbox.zenodo.org
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zenodo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zenodo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zenodo
provider_slug: zenodo
slug: zenodo-domain-security
source_filename: zenodo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zenodo.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: developers.zenodo.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 13:57:49 2026 GMT\n  hsts: false\n- host: sandbox.zenodo.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: zenodo.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenodo/refs/heads/main/security/zenodo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Research
- Open Data
- Repository
- DOI
- Datasets
- Software
- CERN
- OpenAIRE
- InvenioRDM
- Open Science
- Metadata
- Harvesting
---
