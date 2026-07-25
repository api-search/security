---
api_specs:
- filename: logikio-blueprint-export-api-openapi.yml
  format: yaml
  label: Logik.io Blueprint > Export API
  slug: logikio-blueprint-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-blueprint-export-api-openapi.yml
- filename: logikio-blueprint-import-api-openapi.yml
  format: yaml
  label: Logik.io Blueprint > Import API
  slug: logikio-blueprint-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-blueprint-import-api-openapi.yml
- filename: logikio-bom-api-openapi.yml
  format: yaml
  label: Logik.io BOM API
  slug: logikio-bom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-bom-api-openapi.yml
- filename: logikio-configuration-api-openapi.yml
  format: yaml
  label: Logik.io Configuration API
  slug: logikio-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-configuration-api-openapi.yml
- filename: logikio-configuration-v2-api-openapi.yml
  format: yaml
  label: Logik.io Configuration (V2) API
  slug: logikio-configuration-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-configuration-v2-api-openapi.yml
- filename: logikio-managed-tables-export-tables-api-openapi.yml
  format: yaml
  label: Logik.io Managed Tables > Export Tables API
  slug: logikio-managed-tables-export-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-managed-tables-export-tables-api-openapi.yml
- filename: logikio-managed-tables-import-tables-api-openapi.yml
  format: yaml
  label: Logik.io Managed Tables > Import Tables API
  slug: logikio-managed-tables-import-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-managed-tables-import-tables-api-openapi.yml
- filename: logikio-managed-tables-metadata-api-openapi.yml
  format: yaml
  label: Logik.io Managed Tables > Metadata API
  slug: logikio-managed-tables-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-managed-tables-metadata-api-openapi.yml
- filename: logikio-managed-tables-table-rows-api-openapi.yml
  format: yaml
  label: Logik.io Managed Tables > Table Rows API
  slug: logikio-managed-tables-table-rows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-managed-tables-table-rows-api-openapi.yml
- filename: logikio-managed-tables-tables-api-openapi.yml
  format: yaml
  label: Logik.io Managed Tables > Tables API
  slug: logikio-managed-tables-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-managed-tables-tables-api-openapi.yml
- filename: logikio-runtime-bill-of-materials-api-openapi.yml
  format: yaml
  label: Logik.io Runtime - Bill of Materials API
  slug: logikio-runtime-bill-of-materials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-runtime-bill-of-materials-api-openapi.yml
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
