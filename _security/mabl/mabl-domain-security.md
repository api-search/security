---
api_specs:
- filename: mabl-applications-api-openapi.yml
  format: yaml
  label: Mabl Applications API
  slug: mabl-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mabl/refs/heads/main/openapi/mabl-applications-api-openapi.yml
- filename: mabl-credentials-api-openapi.yml
  format: yaml
  label: Mabl Credentials API
  slug: mabl-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mabl/refs/heads/main/openapi/mabl-credentials-api-openapi.yml
- filename: mabl-database-connections-api-openapi.yml
  format: yaml
  label: Mabl Database Connections API
  slug: mabl-database-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mabl/refs/heads/main/openapi/mabl-database-connections-api-openapi.yml
- filename: mabl-deployment-events-api-openapi.yml
  format: yaml
  label: Mabl Deployment Events API
  slug: mabl-deployment-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mabl/refs/heads/main/openapi/mabl-deployment-events-api-openapi.yml
- filename: mabl-environments-api-openapi.yml
  format: yaml
  label: Mabl Environments API
  slug: mabl-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mabl/refs/heads/main/openapi/mabl-environments-api-openapi.yml
- filename: mabl-flows-api-openapi.yml
  format: yaml
  label: Mabl Flows API
  slug: mabl-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mabl/refs/heads/main/openapi/mabl-flows-api-openapi.yml
- filename: mabl-issues-api-openapi.yml
  format: yaml
  label: Mabl Issues API
  slug: mabl-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mabl/refs/heads/main/openapi/mabl-issues-api-openapi.yml
- filename: mabl-test-runs-api-openapi.yml
  format: yaml
  label: Mabl Test Runs API
  slug: mabl-test-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mabl/refs/heads/main/openapi/mabl-test-runs-api-openapi.yml
- filename: mabl-tests-api-openapi.yml
  format: yaml
  label: Mabl Tests API
  slug: mabl-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mabl/refs/heads/main/openapi/mabl-tests-api-openapi.yml
- filename: mabl-users-api-openapi.yml
  format: yaml
  label: Mabl Users API
  slug: mabl-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mabl/refs/heads/main/openapi/mabl-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mabl.com
  spf: true
hosts:
- cert_expires: Sep 21 00:17:03 2026 GMT
  host: www.mabl.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 05:44:53 2026 GMT
  host: mabl.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 10:49:45 2026 GMT
  host: api.mabl.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mabl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mabl, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mabl
provider_slug: mabl
slug: mabl-domain-security
source_filename: mabl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mabl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 00:17:03 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: mabl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 05:44:53 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.mabl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 10:49:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: mabl.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mabl/refs/heads/main/security/mabl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Test Automation
- QA
- DevOps
- AI Testing
- Platform
---
