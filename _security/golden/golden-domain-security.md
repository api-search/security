---
api_specs:
- filename: golden-entity-api-api-openapi.yml
  format: yaml
  label: Golden Entity API API
  slug: golden-entity-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/golden/refs/heads/main/openapi/golden-entity-api-api-openapi.yml
- filename: golden-query-api-api-openapi.yml
  format: yaml
  label: Golden Query API API
  slug: golden-query-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/golden/refs/heads/main/openapi/golden-query-api-api-openapi.yml
- filename: golden-schema-api-api-openapi.yml
  format: yaml
  label: Golden Schema API API
  slug: golden-schema-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/golden/refs/heads/main/openapi/golden-schema-api-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: golden.com
  spf: true
hosts:
- cert_expires: Sep 30 10:58:48 2026 GMT
  host: docs.golden.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 11:52:29 2026 GMT
  host: golden.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Golden Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Golden, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Golden
provider_slug: golden
slug: golden-domain-security
source_filename: golden-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.golden.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 10:58:48 2026 GMT\n  hsts: false\n- host: golden.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 11:52:29 2026 GMT\n  hsts: false\ndomains:\n- domain: golden.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/golden/refs/heads/main/security/golden-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Knowledge Graph
- Company Data
- Data
- Entities
- Artificial Intelligence
- Search
- Business Intelligence
---
