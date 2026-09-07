---
api_specs:
- filename: cancer-gov-seer-openapi.yml
  format: yaml
  label: NCI SEER API
  slug: seer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-seer-openapi.yml
- filename: cancer-gov-modac-openapi.yml
  format: yaml
  label: NCI MoDaC API
  slug: modac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-modac-openapi.yml
- filename: cancer-gov-evs-openapi.yml
  format: yaml
  label: NCI EVS Terminology API
  slug: evs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-evs-openapi.yml
- filename: cancer-gov-diseases-api-openapi.yml
  format: yaml
  label: Cancer.gov Diseases API
  slug: cancer-gov-diseases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-diseases-api-openapi.yml
- filename: cancer-gov-interventions-api-openapi.yml
  format: yaml
  label: Cancer.gov Interventions API
  slug: cancer-gov-interventions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-interventions-api-openapi.yml
- filename: cancer-gov-terms-api-openapi.yml
  format: yaml
  label: Cancer.gov Terms API
  slug: cancer-gov-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-terms-api-openapi.yml
- filename: cancer-gov-trials-api-openapi.yml
  format: yaml
  label: Cancer.gov Trials API
  slug: cancer-gov-trials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-trials-api-openapi.yml
- filename: cancer-gov-glossary-openapi.yml
  format: yaml
  label: NCI Glossary Term API
  slug: glossary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-glossary-openapi.yml
- filename: cancer-gov-drug-dictionary-openapi.yml
  format: yaml
  label: NCI Drug Dictionary API
  slug: drug-dictionary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-drug-dictionary-openapi.yml
- filename: cancer-gov-sitewide-search-openapi.yml
  format: yaml
  label: Cancer.gov Site-Wide Search API
  slug: sitewide-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-sitewide-search-openapi.yml
- filename: cancer-gov-best-bets-openapi.yml
  format: yaml
  label: Cancer.gov Best Bets API
  slug: best-bets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-best-bets-openapi.yml
- filename: cancer-gov-r4r-openapi.yml
  format: yaml
  label: NCI Resources for Researchers API
  slug: r4r-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-r4r-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "entrust.net"
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cancer.gov
  spf: true
hosts:
- cert_expires: Nov 11 12:15:44 2026 GMT
  host: www.cancer.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.cancer.gov
  https: false
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: clinicaltrialsapi.cancer.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Cancer Gov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cancer.gov, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cancer.gov
provider_slug: cancer-gov
slug: cancer-gov-domain-security
source_filename: cancer-gov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cancer.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 12:15:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cancer.gov\n  https: false\n- host: clinicaltrialsapi.cancer.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cancer.gov\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/security/cancer-gov-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cancer
- Federal-Government
- Healthcare
- Research
- Clinical Trials
- Genomics
- Surveillance
- Open Data
---
