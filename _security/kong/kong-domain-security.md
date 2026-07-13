---
api_specs:
- filename: kong-gateway-admin-api.yml
  format: yaml
  label: Kong Gateway Admin API
  slug: kong-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/openapi/kong-gateway-admin-api.yml
- filename: kong-konnect-platform-api.yml
  format: yaml
  label: Kong Konnect Platform API
  slug: kong-konnect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/openapi/kong-konnect-platform-api.yml
- filename: openapi.yaml
  format: yaml
  label: Kong Event Gateway
  slug: kong-event-gateway
  spec_type: OpenAPI
  url: https://developer.konghq.com/api/konnect/event-gateway/v1/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: konghq.com
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: konghq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 00:53:45 2026 GMT
  host: developer.konghq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 19:57:36 2026 GMT
  host: us.api.konghq.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kong Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kong, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Kong
provider_slug: kong
slug: kong-domain-security
source_filename: kong-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: konghq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: false\n- host: developer.konghq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 00:53:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: us.api.konghq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:57:36 2026 GMT\n  hsts: null\ndomains:\n- domain: konghq.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/security/kong-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- API Gateway
- AI Gateway
- AI Connectivity
- Agent Gateway
- Event Gateway
- MCP Registry
- Service Mesh
- LLM
- Kafka
- Konnect
- Open Source
---
