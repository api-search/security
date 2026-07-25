---
api_specs:
- filename: pdb-general-api-openapi.yml
  format: yaml
  label: RCSB PDB General API
  slug: pdb-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdb/refs/heads/main/openapi/pdb-general-api-openapi.yml
- filename: pdb-metadata-service-api-openapi.yml
  format: yaml
  label: RCSB PDB Metadata Service API
  slug: pdb-metadata-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdb/refs/heads/main/openapi/pdb-metadata-service-api-openapi.yml
- filename: pdb-search-service-api-openapi.yml
  format: yaml
  label: RCSB PDB Search Service API
  slug: pdb-search-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdb/refs/heads/main/openapi/pdb-search-service-api-openapi.yml
- filename: pdb-suggest-service-api-openapi.yml
  format: yaml
  label: RCSB PDB Suggest Service API
  slug: pdb-suggest-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdb/refs/heads/main/openapi/pdb-suggest-service-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rcsb.org
  spf: true
hosts:
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: www.rcsb.org
  hsts: true
  hsts_max_age: 16000000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: data.rcsb.org
  hsts: true
  hsts_max_age: 16000000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: search.rcsb.org
  hsts: true
  hsts_max_age: 16000000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pdb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RCSB PDB, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RCSB PDB
provider_slug: pdb
slug: pdb-domain-security
source_filename: pdb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rcsb.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 16000000\n- host: data.rcsb.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 16000000\n- host: search.rcsb.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 16000000\ndomains:\n- domain: rcsb.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pdb/refs/heads/main/security/pdb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Structural Biology
- Proteomics
- Bioinformatics
- Genomics
- Life Sciences
- Open Data
- Research
- Macromolecules
- Crystallography
- NMR
---
