---
api_specs:
- filename: argilla-authentication-api-openapi.yml
  format: yaml
  label: Argilla Authentication API
  slug: argilla-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-authentication-api-openapi.yml
- filename: argilla-datasets-api-openapi.yml
  format: yaml
  label: Argilla datasets API
  slug: argilla-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-datasets-api-openapi.yml
- filename: argilla-fields-api-openapi.yml
  format: yaml
  label: Argilla fields API
  slug: argilla-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-fields-api-openapi.yml
- filename: argilla-info-api-openapi.yml
  format: yaml
  label: Argilla info API
  slug: argilla-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-info-api-openapi.yml
- filename: argilla-jobs-api-openapi.yml
  format: yaml
  label: Argilla jobs API
  slug: argilla-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-jobs-api-openapi.yml
- filename: argilla-metadata-properties-api-openapi.yml
  format: yaml
  label: Argilla metadata properties API
  slug: argilla-metadata-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-metadata-properties-api-openapi.yml
- filename: argilla-questions-api-openapi.yml
  format: yaml
  label: Argilla questions API
  slug: argilla-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-questions-api-openapi.yml
- filename: argilla-records-api-openapi.yml
  format: yaml
  label: Argilla records API
  slug: argilla-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-records-api-openapi.yml
- filename: argilla-responses-api-openapi.yml
  format: yaml
  label: Argilla responses API
  slug: argilla-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-responses-api-openapi.yml
- filename: argilla-settings-api-openapi.yml
  format: yaml
  label: Argilla settings API
  slug: argilla-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-settings-api-openapi.yml
- filename: argilla-suggestions-api-openapi.yml
  format: yaml
  label: Argilla suggestions API
  slug: argilla-suggestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-suggestions-api-openapi.yml
- filename: argilla-users-api-openapi.yml
  format: yaml
  label: Argilla users API
  slug: argilla-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-users-api-openapi.yml
- filename: argilla-vectors-settings-api-openapi.yml
  format: yaml
  label: Argilla vectors-settings API
  slug: argilla-vectors-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-vectors-settings-api-openapi.yml
- filename: argilla-webhooks-api-openapi.yml
  format: yaml
  label: Argilla webhooks API
  slug: argilla-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-webhooks-api-openapi.yml
- filename: argilla-workspaces-api-openapi.yml
  format: yaml
  label: Argilla workspaces API
  slug: argilla-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-workspaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: argilla.io
  spf: true
hosts:
- cert_expires: Aug 28 17:23:51 2026 GMT
  host: argilla.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 18:53:48 2026 GMT
  host: docs.argilla.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Argilla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Argilla, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Argilla
provider_slug: argilla
slug: argilla-domain-security
source_filename: argilla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: argilla.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 17:23:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.argilla.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 18:53:48 2026 GMT\n  hsts: false\ndomains:\n- domain: argilla.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/security/argilla-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- data annotation
- LLM
- NLP
- RLHF
- machine learning
- datasets
- open source
- human feedback
- fine-tuning
- Hugging Face
---
