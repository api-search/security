---
api_specs:
- filename: docs
  format: yaml
  label: ChEMBL Data API
  slug: chembl-data-api
  spec_type: OpenAPI
  url: https://www.ebi.ac.uk/chembl/api/data/docs
- filename: docs
  format: yaml
  label: ChEMBL Cheminformatics Utilities API
  slug: chembl-cheminformatics-utilities-api
  spec_type: OpenAPI
  url: https://www.ebi.ac.uk/chembl/api/utils/docs
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
