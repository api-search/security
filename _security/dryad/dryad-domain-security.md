---
api_specs:
- filename: dryad-datasets-api-openapi.yml
  format: yaml
  label: Dryad datasets API
  slug: dryad-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dryad/refs/heads/main/openapi/dryad-datasets-api-openapi.yml
- filename: dryad-files-api-openapi.yml
  format: yaml
  label: Dryad files API
  slug: dryad-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dryad/refs/heads/main/openapi/dryad-files-api-openapi.yml
- filename: dryad-internal-api-openapi.yml
  format: yaml
  label: Dryad internal API
  slug: dryad-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dryad/refs/heads/main/openapi/dryad-internal-api-openapi.yml
- filename: dryad-reports-api-openapi.yml
  format: yaml
  label: Dryad reports API
  slug: dryad-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dryad/refs/heads/main/openapi/dryad-reports-api-openapi.yml
- filename: dryad-root-api-openapi.yml
  format: yaml
  label: Dryad root API
  slug: dryad-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dryad/refs/heads/main/openapi/dryad-root-api-openapi.yml
- filename: dryad-search-api-openapi.yml
  format: yaml
  label: Dryad search API
  slug: dryad-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dryad/refs/heads/main/openapi/dryad-search-api-openapi.yml
- filename: dryad-versions-api-openapi.yml
  format: yaml
  label: Dryad versions API
  slug: dryad-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dryad/refs/heads/main/openapi/dryad-versions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: datadryad.org
  spf: true
hosts:
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: datadryad.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: sandbox.datadryad.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dryad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dryad, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dryad
provider_slug: dryad
slug: dryad-domain-security
source_filename: dryad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datadryad.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: false\n- host: sandbox.datadryad.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: datadryad.org\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dryad/refs/heads/main/security/dryad-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Research Data
- Open Science
- Data Repository
- Datasets
- Biology
- Ecology
- Open Access
---
