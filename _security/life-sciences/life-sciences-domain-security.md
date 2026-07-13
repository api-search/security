---
api_specs:
- filename: swagger.yaml
  format: yaml
  label: ClinicalTrials.gov API v2
  slug: clinicaltrialsgov-api-v2
  spec_type: OpenAPI
  url: https://clinicaltrials.gov/api/v2/swagger.yaml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "godaddy.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: clinicaltrials.gov
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: euclinicaltrials.eu
  spf: false
hosts:
- cert_expires: Sep 26 14:32:09 2026 GMT
  host: clinicaltrials.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: euclinicaltrials.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 18:57:13 2026 GMT
  host: open.fda.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Life Sciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Life Sciences, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Life Sciences
provider_slug: life-sciences
slug: life-sciences-domain-security
source_filename: life-sciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clinicaltrials.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:32:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: euclinicaltrials.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: open.fda.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:57:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clinicaltrials.gov\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: euclinicaltrials.eu\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/life-sciences/refs/heads/main/security/life-sciences-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Life Sciences
- Biotech
- Pharma
- Healthcare
- Clinical Trials
- Drug Information
- Genomics
- Bioinformatics
- EHR
- FHIR
- Lab Informatics
---
