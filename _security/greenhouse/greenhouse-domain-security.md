---
api_specs:
- filename: greenhouse-harvest-openapi.yml
  format: yaml
  label: Greenhouse Harvest API
  slug: harvest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-harvest-openapi.yml
- filename: greenhouse-job-board-openapi.yml
  format: yaml
  label: Greenhouse Job Board API
  slug: job-board
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-job-board-openapi.yml
- filename: greenhouse-ingestion-openapi.yml
  format: yaml
  label: Greenhouse Candidate Ingestion API
  slug: ingestion
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-ingestion-openapi.yml
- filename: greenhouse-onboarding-openapi.yml
  format: yaml
  label: Greenhouse Onboarding API
  slug: onboarding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-onboarding-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: greenhouse.io
  spf: true
hosts:
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: developers.greenhouse.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: harvest.greenhouse.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: boards-api.greenhouse.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Greenhouse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Greenhouse, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Greenhouse
provider_slug: greenhouse
slug: greenhouse-domain-security
source_filename: greenhouse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.greenhouse.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: false\n- host: harvest.greenhouse.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: null\n- host: boards-api.greenhouse.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: greenhouse.io\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/security/greenhouse-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- ATS
- Recruiting
- Candidates
- Jobs
- Onboarding
- HR
---
