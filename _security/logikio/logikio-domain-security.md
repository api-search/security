---
api_specs:
- filename: logikio-runtime-v2-openapi-original.yml
  format: yaml
  label: Logik Configurator Runtime API (v2)
  slug: logik-configurator-runtime-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-runtime-v2-openapi-original.yml
- filename: logikio-runtime-v1-openapi-original.yml
  format: yaml
  label: Logik Configurator Runtime API (v1)
  slug: logik-configurator-runtime-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-runtime-v1-openapi-original.yml
- filename: logikio-admin-managed-tables-openapi-original.yml
  format: yaml
  label: Logik.io Admin API - Managed Tables
  slug: logikio-admin-api-managed-tables
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-admin-managed-tables-openapi-original.yml
- filename: logikio-admin-blueprint-openapi-original.yml
  format: yaml
  label: Logik.io Admin API - Blueprint Import/Export
  slug: logikio-admin-api-blueprint-importexport
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-admin-blueprint-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 iodef "mailto:security@logik.io"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: logik.io
  spf: true
hosts:
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: www.logik.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Logikio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Logik.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Logik.io
provider_slug: logikio
slug: logikio-domain-security
source_filename: logikio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.logik.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: logik.io\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:security@logik.io\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/security/logikio-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Sales Tech
- CPQ
- Configure Price Quote
- Product Configuration
- Bill of Materials
- Ecommerce
- Salesforce
- API-First
---
