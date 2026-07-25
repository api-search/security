---
api_specs:
- filename: datacite-activities-api-openapi.yml
  format: yaml
  label: DataCite activities API
  slug: datacite-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-activities-api-openapi.yml
- filename: datacite-client-prefixes-api-openapi.yml
  format: yaml
  label: DataCite client-prefixes API
  slug: datacite-client-prefixes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-client-prefixes-api-openapi.yml
- filename: datacite-clients-api-openapi.yml
  format: yaml
  label: DataCite clients API
  slug: datacite-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-clients-api-openapi.yml
- filename: datacite-dois-api-openapi.yml
  format: yaml
  label: DataCite dois API
  slug: datacite-dois-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-dois-api-openapi.yml
- filename: datacite-events-api-openapi.yml
  format: yaml
  label: DataCite events API
  slug: datacite-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-events-api-openapi.yml
- filename: datacite-heartbeat-api-openapi.yml
  format: yaml
  label: DataCite heartbeat API
  slug: datacite-heartbeat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-heartbeat-api-openapi.yml
- filename: datacite-prefixes-api-openapi.yml
  format: yaml
  label: DataCite prefixes API
  slug: datacite-prefixes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-prefixes-api-openapi.yml
- filename: datacite-provider-prefixes-api-openapi.yml
  format: yaml
  label: DataCite provider-prefixes API
  slug: datacite-provider-prefixes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-provider-prefixes-api-openapi.yml
- filename: datacite-providers-api-openapi.yml
  format: yaml
  label: DataCite providers API
  slug: datacite-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-providers-api-openapi.yml
- filename: datacite-publishers-api-openapi.yml
  format: yaml
  label: DataCite publishers API
  slug: datacite-publishers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-publishers-api-openapi.yml
- filename: datacite-report-types-api-openapi.yml
  format: yaml
  label: DataCite report_types API
  slug: datacite-report-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-report-types-api-openapi.yml
- filename: datacite-reports-api-openapi.yml
  format: yaml
  label: DataCite reports API
  slug: datacite-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-reports-api-openapi.yml
- filename: datacite-repositories-api-openapi.yml
  format: yaml
  label: DataCite repositories API
  slug: datacite-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-repositories-api-openapi.yml
- filename: datacite-status-api-openapi.yml
  format: yaml
  label: DataCite status API
  slug: datacite-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: datacite.org
  spf: true
hosts:
- cert_expires: Sep 14 00:27:38 2026 GMT
  host: datacite.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 12:46:16 2026 GMT
  host: support.datacite.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: api.datacite.org
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Datacite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DataCite, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DataCite
provider_slug: datacite
slug: datacite-domain-security
source_filename: datacite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datacite.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 00:27:38 2026 GMT\n  hsts: false\n- host: support.datacite.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 12:46:16 2026 GMT\n  hsts: null\n- host: api.datacite.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: datacite.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/security/datacite-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- DOI
- Persistent Identifiers
- Scholarly Metadata
- Research Data
- Open Science
- Linked Data
---
