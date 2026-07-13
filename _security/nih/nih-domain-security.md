---
api_specs:
- filename: datasets.openapi.yaml
  format: yaml
  label: NCBI Datasets v2 REST API
  slug: ncbi-datasets-v2-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ncbi/datasets/master/datasets.openapi.yaml
- filename: v2
  format: yaml
  label: ClinicalTrials.gov REST API
  slug: clinicaltrialsgov-rest-api
  spec_type: OpenAPI
  url: https://clinicaltrials.gov/api/oas/v2
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "entrust.net"
  - 0 issue "godaddy.com"
  - 0 issue "identrust.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nih.gov
  spf: true
hosts:
- cert_expires: Sep 20 12:45:50 2026 GMT
  host: www.nih.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 14:06:42 2026 GMT
  host: www.ncbi.nlm.nih.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 14:06:42 2026 GMT
  host: eutils.ncbi.nlm.nih.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nih Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Institutes of Health (NIH), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: National Institutes of Health (NIH)
provider_slug: nih
slug: nih-domain-security
source_filename: nih-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nih.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 12:45:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.ncbi.nlm.nih.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:06:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: eutils.ncbi.nlm.nih.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:06:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nih.gov\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"identrust.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nih/refs/heads/main/security/nih-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Biomedical
- Research
- PubMed
- ClinicalTrials
- PubChem
- Genomics
- Health
- Science
- Government
---
