---
api_specs:
- filename: rcsb-pdb-search-api.json
  format: json
  label: RCSB PDB Search API
  slug: rcsb-pdb-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdb/refs/heads/main/openapi/rcsb-pdb-search-api.json
- filename: rcsb-pdb-model-server-api.json
  format: json
  label: RCSB PDB ModelServer API
  slug: rcsb-pdb-model-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdb/refs/heads/main/openapi/rcsb-pdb-model-server-api.json
- filename: rcsb-pdb-volume-server-api.json
  format: json
  label: RCSB PDB VolumeServer API
  slug: rcsb-pdb-volume-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdb/refs/heads/main/openapi/rcsb-pdb-volume-server-api.json
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
