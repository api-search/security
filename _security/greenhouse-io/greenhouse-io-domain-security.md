---
api_specs:
- filename: greenhouse-harvest-api-openapi.yml
  format: yaml
  label: Greenhouse Harvest API
  slug: greenhouse-harvest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse-io/refs/heads/main/openapi/greenhouse-harvest-api-openapi.yml
- filename: greenhouse-job-board-api-openapi.yml
  format: yaml
  label: Greenhouse Job Board API
  slug: greenhouse-job-board-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse-io/refs/heads/main/openapi/greenhouse-job-board-api-openapi.yml
- filename: greenhouse-audit-log-api-openapi.yml
  format: yaml
  label: Greenhouse Audit Log API
  slug: greenhouse-audit-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse-io/refs/heads/main/openapi/greenhouse-audit-log-api-openapi.yml
- filename: greenhouse-candidate-ingestion-api-openapi.yml
  format: yaml
  label: Greenhouse Candidate Ingestion (Partner) API
  slug: greenhouse-candidate-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse-io/refs/heads/main/openapi/greenhouse-candidate-ingestion-api-openapi.yml
- filename: greenhouse-onboarding-api-openapi.yml
  format: yaml
  label: Greenhouse Onboarding API
  slug: greenhouse-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse-io/refs/heads/main/openapi/greenhouse-onboarding-api-openapi.yml
- filename: greenhouse-assessment-api-openapi.yml
  format: yaml
  label: Greenhouse Assessment Partner API
  slug: greenhouse-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse-io/refs/heads/main/openapi/greenhouse-assessment-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: greenhouse.com
  spf: true
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: greenhouse.io
  spf: true
hosts:
- cert_expires: Aug 25 23:27:17 2026 GMT
  host: www.greenhouse.com
  hsts: false
  https: true
  tls_version: TLSv1.3
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
kind: domain-security
layout: security
method: probed
name: Greenhouse Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Greenhouse, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Greenhouse
provider_slug: greenhouse-io
slug: greenhouse-io-domain-security
source_filename: greenhouse-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.greenhouse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:27:17 2026 GMT\n  hsts: false\n- host: developers.greenhouse.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: false\n- host: harvest.greenhouse.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: greenhouse.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: greenhouse.io\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\
  \n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greenhouse-io/refs/heads/main/security/greenhouse-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- ATS
- Recruiting
- Hiring
- Talent Acquisition
- Enterprise SaaS
- Human Resources
- Onboarding
---
