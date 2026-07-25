---
api_specs:
- filename: chembl-activity-api-openapi.yml
  format: yaml
  label: ChEMBL Activity API
  slug: chembl-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-activity-api-openapi.yml
- filename: chembl-assay-api-openapi.yml
  format: yaml
  label: ChEMBL Assay API
  slug: chembl-assay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-assay-api-openapi.yml
- filename: chembl-atc-classification-api-openapi.yml
  format: yaml
  label: ChEMBL ATC Classification API
  slug: chembl-atc-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-atc-classification-api-openapi.yml
- filename: chembl-binding-site-api-openapi.yml
  format: yaml
  label: ChEMBL Binding Site API
  slug: chembl-binding-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-binding-site-api-openapi.yml
- filename: chembl-cell-line-api-openapi.yml
  format: yaml
  label: ChEMBL Cell Line API
  slug: chembl-cell-line-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-cell-line-api-openapi.yml
- filename: chembl-compound-record-api-openapi.yml
  format: yaml
  label: ChEMBL Compound Record API
  slug: chembl-compound-record-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-compound-record-api-openapi.yml
- filename: chembl-document-api-openapi.yml
  format: yaml
  label: ChEMBL Document API
  slug: chembl-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-document-api-openapi.yml
- filename: chembl-drug-api-openapi.yml
  format: yaml
  label: ChEMBL Drug API
  slug: chembl-drug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-drug-api-openapi.yml
- filename: chembl-drug-indication-api-openapi.yml
  format: yaml
  label: ChEMBL Drug Indication API
  slug: chembl-drug-indication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-drug-indication-api-openapi.yml
- filename: chembl-drug-warning-api-openapi.yml
  format: yaml
  label: ChEMBL Drug Warning API
  slug: chembl-drug-warning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-drug-warning-api-openapi.yml
- filename: chembl-mechanism-api-openapi.yml
  format: yaml
  label: ChEMBL Mechanism API
  slug: chembl-mechanism-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-mechanism-api-openapi.yml
- filename: chembl-molecule-api-openapi.yml
  format: yaml
  label: ChEMBL Molecule API
  slug: chembl-molecule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-molecule-api-openapi.yml
- filename: chembl-similarity-api-openapi.yml
  format: yaml
  label: ChEMBL Similarity API
  slug: chembl-similarity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-similarity-api-openapi.yml
- filename: chembl-status-api-openapi.yml
  format: yaml
  label: ChEMBL Status API
  slug: chembl-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-status-api-openapi.yml
- filename: chembl-substructure-api-openapi.yml
  format: yaml
  label: ChEMBL Substructure API
  slug: chembl-substructure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-substructure-api-openapi.yml
- filename: chembl-target-api-openapi.yml
  format: yaml
  label: ChEMBL Target API
  slug: chembl-target-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-target-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gitbook.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ebi.ac.uk
  spf: true
hosts:
- cert_expires: Aug 17 17:00:10 2026 GMT
  host: chembl.gitbook.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: www.ebi.ac.uk
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chembl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChEMBL, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ChEMBL
provider_slug: chembl
slug: chembl-domain-security
source_filename: chembl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chembl.gitbook.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 17:00:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.ebi.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: gitbook.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ebi.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/security/chembl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Drug Discovery
- Bioactivity
- Molecules
- Cheminformatics
- Life Sciences
- Bioinformatics
- Pharmacology
- EMBL-EBI
---
