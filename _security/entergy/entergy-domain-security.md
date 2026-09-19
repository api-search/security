---
api_specs:
- filename: entergy-mdd-pro-v2-api-openapi.yml
  format: yaml
  label: Entergy Mdd Pro/v2 API
  slug: entergy-mdd-pro-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergy/refs/heads/main/openapi/entergy-mdd-pro-v2-api-openapi.yml
- filename: entergy-oembed-1-0-api-openapi.yml
  format: yaml
  label: Entergy Oembed/1.0 API
  slug: entergy-oembed-1-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergy/refs/heads/main/openapi/entergy-oembed-1-0-api-openapi.yml
- filename: entergy-wp-abilities-v1-api-openapi.yml
  format: yaml
  label: Entergy Wp Abilities/v1 API
  slug: entergy-wp-abilities-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergy/refs/heads/main/openapi/entergy-wp-abilities-v1-api-openapi.yml
- filename: entergy-wp-api-openapi.yml
  format: yaml
  label: Entergy Wp API
  slug: entergy-wp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergy/refs/heads/main/openapi/entergy-wp-api-openapi.yml
- filename: entergy-wp-block-editor-v1-api-openapi.yml
  format: yaml
  label: Entergy Wp Block Editor/v1 API
  slug: entergy-wp-block-editor-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergy/refs/heads/main/openapi/entergy-wp-block-editor-v1-api-openapi.yml
- filename: entergy-wp-site-health-v1-api-openapi.yml
  format: yaml
  label: Entergy Wp Site Health/v1 API
  slug: entergy-wp-site-health-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergy/refs/heads/main/openapi/entergy-wp-site-health-v1-api-openapi.yml
- filename: entergy-wp-v2-api-openapi.yml
  format: yaml
  label: Entergy Wp/v2 API
  slug: entergy-wp-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergy/refs/heads/main/openapi/entergy-wp-v2-api-openapi.yml
- filename: entergy-wpe-cache-plugin-v1-api-openapi.yml
  format: yaml
  label: Entergy Wpe/cache Plugin/v1 API
  slug: entergy-wpe-cache-plugin-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergy/refs/heads/main/openapi/entergy-wpe-cache-plugin-v1-api-openapi.yml
- filename: entergy-wpe-sign-on-plugin-v1-api-openapi.yml
  format: yaml
  label: Entergy Wpe Sign On Plugin/v1 API
  slug: entergy-wpe-sign-on-plugin-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergy/refs/heads/main/openapi/entergy-wpe-sign-on-plugin-v1-api-openapi.yml
- filename: entergy-wpsl-v1-api-openapi.yml
  format: yaml
  label: Entergy Wpsl/v1 API
  slug: entergy-wpsl-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergy/refs/heads/main/openapi/entergy-wpsl-v1-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: entergy.com
  spf: true
hosts:
- cert_expires: Nov 13 16:18:48 2026 GMT
  host: www.entergy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Entergy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Entergy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Entergy
provider_slug: entergy
slug: entergy-domain-security
source_filename: entergy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.entergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 16:18:48 2026 GMT\n  hsts: null\ndomains:\n- domain: entergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/entergy/refs/heads/main/security/entergy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Electricity
- Energy
- Fortune 500
- Utility
- Nuclear
- Power Generation
- Louisiana
- Geospatial
---
