---
api_specs:
- filename: oracle-apex-autorest-api-openapi.yml
  format: yaml
  label: Oracle APEX AutoREST API
  slug: oracle-apex-autorest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-autorest-api-openapi.yml
- filename: oracle-apex-handlers-api-openapi.yml
  format: yaml
  label: Oracle APEX Handlers API
  slug: oracle-apex-handlers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-handlers-api-openapi.yml
- filename: oracle-apex-modules-api-openapi.yml
  format: yaml
  label: Oracle APEX Modules API
  slug: oracle-apex-modules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-modules-api-openapi.yml
- filename: oracle-apex-oauth-clients-api-openapi.yml
  format: yaml
  label: Oracle APEX OAuth Clients API
  slug: oracle-apex-oauth-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-oauth-clients-api-openapi.yml
- filename: oracle-apex-overview-api-openapi.yml
  format: yaml
  label: Oracle APEX Overview API
  slug: oracle-apex-overview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-overview-api-openapi.yml
- filename: oracle-apex-parameters-api-openapi.yml
  format: yaml
  label: Oracle APEX Parameters API
  slug: oracle-apex-parameters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-parameters-api-openapi.yml
- filename: oracle-apex-privileges-api-openapi.yml
  format: yaml
  label: Oracle APEX Privileges API
  slug: oracle-apex-privileges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-privileges-api-openapi.yml
- filename: oracle-apex-properties-api-openapi.yml
  format: yaml
  label: Oracle APEX Properties API
  slug: oracle-apex-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-properties-api-openapi.yml
- filename: oracle-apex-roles-api-openapi.yml
  format: yaml
  label: Oracle APEX Roles API
  slug: oracle-apex-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-roles-api-openapi.yml
- filename: oracle-apex-templates-api-openapi.yml
  format: yaml
  label: Oracle APEX Templates API
  slug: oracle-apex-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-templates-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oracle.com
  spf: true
hosts:
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: apex.oracle.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: www.oracle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: docs.oracle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oracle Apex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oracle APEX, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oracle APEX
provider_slug: oracle-apex
slug: oracle-apex-domain-security
source_filename: oracle-apex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apex.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: null\n- host: www.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: oracle.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/security/oracle-apex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- APEX
- Cloud
- Database
- Development Platform
- Enterprise
- Generative AI
- Low-Code
- Oracle
- ORDS
- PL/SQL
- REST API
- Web Applications
- Workflow
---
