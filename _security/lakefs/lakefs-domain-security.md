---
api_specs:
- filename: lakefs-actions-api-openapi.yml
  format: yaml
  label: lakeFS actions API
  slug: lakefs-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-actions-api-openapi.yml
- filename: lakefs-auth-api-openapi.yml
  format: yaml
  label: lakeFS auth API
  slug: lakefs-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-auth-api-openapi.yml
- filename: lakefs-branches-api-openapi.yml
  format: yaml
  label: lakeFS branches API
  slug: lakefs-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-branches-api-openapi.yml
- filename: lakefs-commits-api-openapi.yml
  format: yaml
  label: lakeFS commits API
  slug: lakefs-commits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-commits-api-openapi.yml
- filename: lakefs-config-api-openapi.yml
  format: yaml
  label: lakeFS config API
  slug: lakefs-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-config-api-openapi.yml
- filename: lakefs-experimental-api-openapi.yml
  format: yaml
  label: lakeFS experimental API
  slug: lakefs-experimental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-experimental-api-openapi.yml
- filename: lakefs-external-api-openapi.yml
  format: yaml
  label: lakeFS external API
  slug: lakefs-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-external-api-openapi.yml
- filename: lakefs-healthcheck-api-openapi.yml
  format: yaml
  label: lakeFS healthCheck API
  slug: lakefs-healthcheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-healthcheck-api-openapi.yml
- filename: lakefs-import-api-openapi.yml
  format: yaml
  label: lakeFS import API
  slug: lakefs-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-import-api-openapi.yml
- filename: lakefs-internal-api-openapi.yml
  format: yaml
  label: lakeFS internal API
  slug: lakefs-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-internal-api-openapi.yml
- filename: lakefs-metadata-api-openapi.yml
  format: yaml
  label: lakeFS metadata API
  slug: lakefs-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-metadata-api-openapi.yml
- filename: lakefs-objects-api-openapi.yml
  format: yaml
  label: lakeFS objects API
  slug: lakefs-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-objects-api-openapi.yml
- filename: lakefs-pulls-api-openapi.yml
  format: yaml
  label: lakeFS pulls API
  slug: lakefs-pulls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-pulls-api-openapi.yml
- filename: lakefs-refs-api-openapi.yml
  format: yaml
  label: lakeFS refs API
  slug: lakefs-refs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-refs-api-openapi.yml
- filename: lakefs-repositories-api-openapi.yml
  format: yaml
  label: lakeFS repositories API
  slug: lakefs-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-repositories-api-openapi.yml
- filename: lakefs-staging-api-openapi.yml
  format: yaml
  label: lakeFS staging API
  slug: lakefs-staging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-staging-api-openapi.yml
- filename: lakefs-tags-api-openapi.yml
  format: yaml
  label: lakeFS tags API
  slug: lakefs-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-tags-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lakefs.io
  spf: true
hosts:
- cert_expires: Aug 22 06:36:06 2026 GMT
  host: lakefs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lakefs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for lakeFS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: lakeFS
provider_slug: lakefs
slug: lakefs-domain-security
source_filename: lakefs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lakefs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 06:36:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lakefs.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/security/lakefs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Version Control
- Data Lake
- Git-like
- Open Source
---
