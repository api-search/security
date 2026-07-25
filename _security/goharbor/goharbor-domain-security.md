---
api_specs:
- filename: goharbor-artifacts-api-openapi.yml
  format: yaml
  label: GoHarbor artifacts API
  slug: goharbor-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-artifacts-api-openapi.yml
- filename: goharbor-audit-api-openapi.yml
  format: yaml
  label: GoHarbor audit API
  slug: goharbor-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-audit-api-openapi.yml
- filename: goharbor-health-api-openapi.yml
  format: yaml
  label: GoHarbor health API
  slug: goharbor-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-health-api-openapi.yml
- filename: goharbor-projects-api-openapi.yml
  format: yaml
  label: GoHarbor projects API
  slug: goharbor-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-projects-api-openapi.yml
- filename: goharbor-quotas-api-openapi.yml
  format: yaml
  label: GoHarbor quotas API
  slug: goharbor-quotas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-quotas-api-openapi.yml
- filename: goharbor-registries-api-openapi.yml
  format: yaml
  label: GoHarbor registries API
  slug: goharbor-registries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-registries-api-openapi.yml
- filename: goharbor-replication-api-openapi.yml
  format: yaml
  label: GoHarbor replication API
  slug: goharbor-replication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-replication-api-openapi.yml
- filename: goharbor-repositories-api-openapi.yml
  format: yaml
  label: GoHarbor repositories API
  slug: goharbor-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-repositories-api-openapi.yml
- filename: goharbor-robots-api-openapi.yml
  format: yaml
  label: GoHarbor robots API
  slug: goharbor-robots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-robots-api-openapi.yml
- filename: goharbor-scan-api-openapi.yml
  format: yaml
  label: GoHarbor scan API
  slug: goharbor-scan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-scan-api-openapi.yml
- filename: goharbor-search-api-openapi.yml
  format: yaml
  label: GoHarbor search API
  slug: goharbor-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-search-api-openapi.yml
- filename: goharbor-tags-api-openapi.yml
  format: yaml
  label: GoHarbor tags API
  slug: goharbor-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-tags-api-openapi.yml
- filename: goharbor-usergroups-api-openapi.yml
  format: yaml
  label: GoHarbor usergroups API
  slug: goharbor-usergroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-usergroups-api-openapi.yml
- filename: goharbor-webhooks-api-openapi.yml
  format: yaml
  label: GoHarbor webhooks API
  slug: goharbor-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: goharbor.io
  spf: false
hosts:
- cert_expires: Aug 24 21:18:45 2026 GMT
  host: goharbor.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Goharbor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoHarbor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: GoHarbor
provider_slug: goharbor
slug: goharbor-domain-security
source_filename: goharbor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goharbor.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 21:18:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: goharbor.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/security/goharbor-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Container Registry
---
