---
api_specs:
- filename: chembl-activities-api-openapi.yml
  format: yaml
  label: ChEMBL Activities API
  slug: chembl-activities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chembl/openapi/chembl-activities-api-openapi.yml
- filename: chembl-assays-api-openapi.yml
  format: yaml
  label: ChEMBL Assays API
  slug: chembl-assays-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chembl/openapi/chembl-assays-api-openapi.yml
- filename: chembl-drugs-api-openapi.yml
  format: yaml
  label: ChEMBL Drugs API
  slug: chembl-drugs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chembl/openapi/chembl-drugs-api-openapi.yml
- filename: chembl-efo-disease-terms-api-openapi.yml
  format: yaml
  label: ChEMBL EFO disease terms API
  slug: chembl-efo-disease-terms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chembl/openapi/chembl-efo-disease-terms-api-openapi.yml
- filename: chembl-hpo-api-openapi.yml
  format: yaml
  label: ChEMBL HPO API
  slug: chembl-hpo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chembl/openapi/chembl-hpo-api-openapi.yml
- filename: chembl-intact-api-openapi.yml
  format: yaml
  label: ChEMBL Intact API
  slug: chembl-intact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chembl/openapi/chembl-intact-api-openapi.yml
- filename: chembl-molecules-api-openapi.yml
  format: yaml
  label: ChEMBL Molecules API
  slug: chembl-molecules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chembl/openapi/chembl-molecules-api-openapi.yml
- filename: chembl-proteins-api-openapi.yml
  format: yaml
  label: ChEMBL Proteins API
  slug: chembl-proteins-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chembl/openapi/chembl-proteins-api-openapi.yml
- filename: chembl-pubchem-bioassay-sids-api-openapi.yml
  format: yaml
  label: ChEMBL PubChem Bioassay Sids API
  slug: chembl-pubchem-bioassay-sids-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chembl/openapi/chembl-pubchem-bioassay-sids-api-openapi.yml
- filename: chembl-pubchem-biossays-api-openapi.yml
  format: yaml
  label: ChEMBL PubChem Biossays API
  slug: chembl-pubchem-biossays-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chembl/openapi/chembl-pubchem-biossays-api-openapi.yml
- filename: chembl-pubchem-compounds-api-openapi.yml
  format: yaml
  label: ChEMBL PubChem Compounds API
  slug: chembl-pubchem-compounds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chembl/openapi/chembl-pubchem-compounds-api-openapi.yml
- filename: chembl-pubchem-substances-api-openapi.yml
  format: yaml
  label: ChEMBL PubChem Substances API
  slug: chembl-pubchem-substances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chembl/openapi/chembl-pubchem-substances-api-openapi.yml
- filename: chembl-targets-api-openapi.yml
  format: yaml
  label: ChEMBL Targets API
  slug: chembl-targets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chembl/openapi/chembl-targets-api-openapi.yml
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
hosts_probed: 2
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
source_yaml_url: https://artifacts.apis.io/chembl/security/chembl-domain-security.yml
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
