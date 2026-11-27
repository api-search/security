---
api_specs:
- filename: movahedi-ca-breach-deadlines-api-openapi.yml
  format: yaml
  label: Mohammad Movahedi Breach Deadlines API
  slug: movahedi-ca-breach-deadlines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movahedi-ca/openapi/movahedi-ca-breach-deadlines-api-openapi.yml
- filename: movahedi-ca-cookies-api-openapi.yml
  format: yaml
  label: Mohammad Movahedi Cookies API
  slug: movahedi-ca-cookies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movahedi-ca/openapi/movahedi-ca-cookies-api-openapi.yml
- filename: movahedi-ca-crawlers-api-openapi.yml
  format: yaml
  label: Mohammad Movahedi Crawlers API
  slug: movahedi-ca-crawlers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movahedi-ca/openapi/movahedi-ca-crawlers-api-openapi.yml
- filename: movahedi-ca-enforcement-api-openapi.yml
  format: yaml
  label: Mohammad Movahedi Enforcement API
  slug: movahedi-ca-enforcement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movahedi-ca/openapi/movahedi-ca-enforcement-api-openapi.yml
- filename: movahedi-ca-glossary-api-openapi.yml
  format: yaml
  label: Mohammad Movahedi Glossary API
  slug: movahedi-ca-glossary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movahedi-ca/openapi/movahedi-ca-glossary-api-openapi.yml
- filename: movahedi-ca-health-api-openapi.yml
  format: yaml
  label: Mohammad Movahedi Health API
  slug: movahedi-ca-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movahedi-ca/openapi/movahedi-ca-health-api-openapi.yml
- filename: movahedi-ca-law25-api-openapi.yml
  format: yaml
  label: Mohammad Movahedi Law25 API
  slug: movahedi-ca-law25-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movahedi-ca/openapi/movahedi-ca-law25-api-openapi.yml
- filename: movahedi-ca-openapi-json-api-openapi.yml
  format: yaml
  label: Mohammad Movahedi Openapi.json API
  slug: movahedi-ca-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movahedi-ca/openapi/movahedi-ca-openapi-json-api-openapi.yml
- filename: movahedi-ca-terms-api-openapi.yml
  format: yaml
  label: Mohammad Movahedi Terms API
  slug: movahedi-ca-terms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movahedi-ca/openapi/movahedi-ca-terms-api-openapi.yml
- filename: movahedi-ca-vm-health-api-openapi.yml
  format: yaml
  label: Mohammad Movahedi Vm Health API
  slug: movahedi-ca-vm-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movahedi-ca/openapi/movahedi-ca-vm-health-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: movahedi.ca
  spf: true
hosts:
- cert_expires: Feb  9 02:49:25 2027 GMT
  host: movahedi.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mohammad Movahedi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mohammad Movahedi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Mohammad Movahedi
provider_slug: movahedi-ca
slug: movahedi-ca-domain-security
source_filename: movahedi-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: movahedi.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 02:49:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: movahedi.ca\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/movahedi-ca/security/movahedi-ca-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Privacy
- AI Governance
- Consulting
- Mississauga
- Canada
---
