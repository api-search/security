---
api_specs:
- filename: volumental-auth-api-openapi.yml
  format: yaml
  label: Volumental Auth API
  slug: volumental-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volumental/refs/heads/main/openapi/volumental-auth-api-openapi.yml
- filename: volumental-oauth-api-openapi.yml
  format: yaml
  label: Volumental OAuth API
  slug: volumental-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volumental/refs/heads/main/openapi/volumental-oauth-api-openapi.yml
- filename: volumental-recommendations-api-openapi.yml
  format: yaml
  label: Volumental Recommendations API
  slug: volumental-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volumental/refs/heads/main/openapi/volumental-recommendations-api-openapi.yml
- filename: volumental-scans-api-openapi.yml
  format: yaml
  label: Volumental Scans API
  slug: volumental-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volumental/refs/heads/main/openapi/volumental-scans-api-openapi.yml
- filename: volumental-some-endpoint-api-openapi.yml
  format: yaml
  label: Volumental Some Endpoint API
  slug: volumental-some-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volumental/refs/heads/main/openapi/volumental-some-endpoint-api-openapi.yml
- filename: volumental-v1alpha-api-openapi.yml
  format: yaml
  label: Volumental V1Alpha API
  slug: volumental-v1alpha-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volumental/refs/heads/main/openapi/volumental-v1alpha-api-openapi.yml
- filename: volumental-v1beta-api-openapi.yml
  format: yaml
  label: Volumental V1Beta API
  slug: volumental-v1beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volumental/refs/heads/main/openapi/volumental-v1beta-api-openapi.yml
- filename: volumental-volumental-api-api-openapi.yml
  format: yaml
  label: Volumental Volumental API
  slug: volumental-volumental-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volumental/refs/heads/main/openapi/volumental-volumental-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: volumental.com
  spf: true
hosts:
- cert_expires: Dec 13 16:35:06 2026 GMT
  host: volumental.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Volumental Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Volumental, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Volumental
provider_slug: volumental
slug: volumental-domain-security
source_filename: volumental-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: volumental.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 16:35:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: volumental.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/volumental/refs/heads/main/security/volumental-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Retail
- Footwear
- 3DScanning
- Artificial Intelligence
---
