---
api_specs:
- filename: clinical-trials-gov-data-api-v2-openapi.yml
  format: yaml
  label: ClinicalTrials.gov Data API v2
  slug: data-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clinical-trials-gov/refs/heads/main/openapi/clinical-trials-gov-data-api-v2-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: clinicaltrials.gov
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: ctti-clinicaltrials.org
  spf: false
hosts:
- cert_expires: Sep 26 14:32:09 2026 GMT
  host: clinicaltrials.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 06:43:37 2026 GMT
  host: aact.ctti-clinicaltrials.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clinical Trials Gov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClinicalTrials.gov, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ClinicalTrials.gov
provider_slug: clinical-trials-gov
slug: clinical-trials-gov-domain-security
source_filename: clinical-trials-gov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clinicaltrials.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:32:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: aact.ctti-clinicaltrials.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 06:43:37 2026 GMT\n  hsts: false\ndomains:\n- domain: clinicaltrials.gov\n  dnssec: true\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ctti-clinicaltrials.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clinical-trials-gov/refs/heads/main/security/clinical-trials-gov-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Clinical Trials
- Government
- Health
- NIH
- Open Data
- Public Health
- Research
---
