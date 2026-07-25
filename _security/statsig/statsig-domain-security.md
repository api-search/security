---
api_specs:
- filename: statsig-events-api-openapi.yml
  format: yaml
  label: Statsig Events API
  slug: events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-events-api-openapi.yml
- filename: statsig-audit-logs-api-openapi.yml
  format: yaml
  label: statsig Audit Logs API
  slug: statsig-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-audit-logs-api-openapi.yml
- filename: statsig-autotunes-api-openapi.yml
  format: yaml
  label: statsig Autotunes API
  slug: statsig-autotunes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-autotunes-api-openapi.yml
- filename: statsig-configuration-api-openapi.yml
  format: yaml
  label: statsig Configuration API
  slug: statsig-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-configuration-api-openapi.yml
- filename: statsig-dynamic-configs-api-openapi.yml
  format: yaml
  label: statsig Dynamic Configs API
  slug: statsig-dynamic-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-dynamic-configs-api-openapi.yml
- filename: statsig-experiments-api-openapi.yml
  format: yaml
  label: statsig Experiments API
  slug: statsig-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-experiments-api-openapi.yml
- filename: statsig-feature-gates-api-openapi.yml
  format: yaml
  label: statsig Feature Gates API
  slug: statsig-feature-gates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-feature-gates-api-openapi.yml
- filename: statsig-gates-api-openapi.yml
  format: yaml
  label: statsig Gates API
  slug: statsig-gates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-gates-api-openapi.yml
- filename: statsig-holdouts-api-openapi.yml
  format: yaml
  label: statsig Holdouts API
  slug: statsig-holdouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-holdouts-api-openapi.yml
- filename: statsig-initialization-api-openapi.yml
  format: yaml
  label: statsig Initialization API
  slug: statsig-initialization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-initialization-api-openapi.yml
- filename: statsig-keys-api-openapi.yml
  format: yaml
  label: statsig Keys API
  slug: statsig-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-keys-api-openapi.yml
- filename: statsig-layers-api-openapi.yml
  format: yaml
  label: statsig Layers API
  slug: statsig-layers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-layers-api-openapi.yml
- filename: statsig-metrics-api-openapi.yml
  format: yaml
  label: statsig Metrics API
  slug: statsig-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-metrics-api-openapi.yml
- filename: statsig-segments-api-openapi.yml
  format: yaml
  label: statsig Segments API
  slug: statsig-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-segments-api-openapi.yml
- filename: statsig-tags-api-openapi.yml
  format: yaml
  label: statsig Tags API
  slug: statsig-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-tags-api-openapi.yml
- filename: statsig-target-apps-api-openapi.yml
  format: yaml
  label: statsig Target Apps API
  slug: statsig-target-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-target-apps-api-openapi.yml
- filename: statsig-users-api-openapi.yml
  format: yaml
  label: statsig Users API
  slug: statsig-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-users-api-openapi.yml
- filename: statsig-webhooks-api-openapi.yml
  format: yaml
  label: statsig Webhooks API
  slug: statsig-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: statsig.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: statsigapi.net
  spf: false
hosts:
- cert_expires: Sep 15 16:23:32 2026 GMT
  host: docs.statsig.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 17:15:26 2026 GMT
  host: api.statsig.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 12:30:25 2026 GMT
  host: statsigapi.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Statsig Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for statsig, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: statsig
provider_slug: statsig
slug: statsig-domain-security
source_filename: statsig-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.statsig.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 16:23:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.statsig.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 17:15:26 2026 GMT\n  hsts: null\n- host: statsigapi.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 12:30:25 2026 GMT\n  hsts: null\ndomains:\n- domain: statsig.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: statsigapi.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/security/statsig-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
