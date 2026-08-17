---
api_specs:
- filename: golden-recursion-entity-api-api-openapi.yml
  format: yaml
  label: Golden Recursion Entity API API
  slug: golden-recursion-entity-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/golden-recursion/refs/heads/main/openapi/golden-recursion-entity-api-api-openapi.yml
- filename: golden-recursion-query-api-api-openapi.yml
  format: yaml
  label: Golden Recursion Query API API
  slug: golden-recursion-query-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/golden-recursion/refs/heads/main/openapi/golden-recursion-query-api-api-openapi.yml
- filename: golden-recursion-schema-api-api-openapi.yml
  format: yaml
  label: Golden Recursion Schema API API
  slug: golden-recursion-schema-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/golden-recursion/refs/heads/main/openapi/golden-recursion-schema-api-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:hello@golden-support.com"
  - 0 issue "comodoca.com"
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
name: Golden Recursion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Golden Recursion, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Golden Recursion
provider_slug: golden-recursion
slug: golden-recursion-domain-security
source_filename: golden-recursion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.golden.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 10:58:48 2026 GMT\n  hsts: false\n- host: golden.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 11:52:29 2026 GMT\n  hsts: false\ndomains:\n- domain: golden.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:hello@golden-support.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/golden-recursion/refs/heads/main/security/golden-recursion-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Knowledge Graph
- Data Enrichment
- Entity Data
- Company Data
- Artificial Intelligence
- Semantic Web
- Data
---
