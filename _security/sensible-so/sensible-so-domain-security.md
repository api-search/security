---
api_specs:
- filename: sensible-so-configuration-api-openapi.yml
  format: yaml
  label: sensible-so Configuration API
  slug: sensible-so-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-so/refs/heads/main/openapi/sensible-so-configuration-api-openapi.yml
- filename: sensible-so-document-api-openapi.yml
  format: yaml
  label: sensible-so Document API
  slug: sensible-so-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-so/refs/heads/main/openapi/sensible-so-document-api-openapi.yml
- filename: sensible-so-document-type-api-openapi.yml
  format: yaml
  label: sensible-so Document type API
  slug: sensible-so-document-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-so/refs/heads/main/openapi/sensible-so-document-type-api-openapi.yml
- filename: sensible-so-get-excel-from-documents-api-openapi.yml
  format: yaml
  label: sensible-so Get Excel from documents API
  slug: sensible-so-get-excel-from-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-so/refs/heads/main/openapi/sensible-so-get-excel-from-documents-api-openapi.yml
- filename: sensible-so-portfolio-api-openapi.yml
  format: yaml
  label: sensible-so Portfolio API
  slug: sensible-so-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-so/refs/heads/main/openapi/sensible-so-portfolio-api-openapi.yml
- filename: sensible-so-reference-document-api-openapi.yml
  format: yaml
  label: sensible-so Reference document API
  slug: sensible-so-reference-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-so/refs/heads/main/openapi/sensible-so-reference-document-api-openapi.yml
- filename: sensible-so-retrieve-extractions-api-openapi.yml
  format: yaml
  label: sensible-so Retrieve extractions API
  slug: sensible-so-retrieve-extractions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-so/refs/heads/main/openapi/sensible-so-retrieve-extractions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sensible.so
  spf: true
hosts:
- cert_expires: Sep 10 07:22:36 2026 GMT
  host: www.sensible.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 20:47:53 2026 GMT
  host: docs.sensible.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: api.sensible.so
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sensible So Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for sensible-so, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: sensible-so
provider_slug: sensible-so
slug: sensible-so-domain-security
source_filename: sensible-so-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sensible.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 07:22:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sensible.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 20:47:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sensible.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sensible.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sensible-so/refs/heads/main/security/sensible-so-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
