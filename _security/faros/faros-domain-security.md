---
api_specs:
- filename: faros-openapi.yml
  format: yaml
  label: Faros Events / Ingestion API (REST)
  slug: faros-events-ingestion-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/faros/refs/heads/main/openapi/faros-openapi.yml
- filename: faros-openapi.yml
  format: yaml
  label: Faros GraphQL Query API
  slug: faros-graphql-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/faros/refs/heads/main/openapi/faros-openapi.yml
- filename: faros-openapi.yml
  format: yaml
  label: Faros Deployments / CI-CD API
  slug: faros-deployments-ci-cd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/faros/refs/heads/main/openapi/faros-openapi.yml
- filename: faros-openapi.yml
  format: yaml
  label: Faros Webhooks API
  slug: faros-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/faros/refs/heads/main/openapi/faros-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: faros.ai
  spf: true
hosts:
- cert_expires: Aug 31 09:17:28 2026 GMT
  host: www.faros.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 04:44:26 2026 GMT
  host: docs.faros.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: prod.api.faros.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Faros Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Faros AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Faros AI
provider_slug: faros
slug: faros-domain-security
source_filename: faros-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.faros.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 09:17:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.faros.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 04:44:26 2026 GMT\n  hsts: null\n- host: prod.api.faros.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: faros.ai\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/faros/refs/heads/main/security/faros-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Engineering Operations
- Software Engineering Intelligence
- SEI
- DORA Metrics
- Developer Productivity
- Data Ingestion
---
