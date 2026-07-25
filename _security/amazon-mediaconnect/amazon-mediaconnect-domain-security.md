---
api_specs:
- filename: amazon-mediaconnect-bridges-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Bridges API
  slug: amazon-mediaconnect-bridges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/openapi/amazon-mediaconnect-bridges-api-openapi.yml
- filename: amazon-mediaconnect-entitlements-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Entitlements API
  slug: amazon-mediaconnect-entitlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/openapi/amazon-mediaconnect-entitlements-api-openapi.yml
- filename: amazon-mediaconnect-flows-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Flows API
  slug: amazon-mediaconnect-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/openapi/amazon-mediaconnect-flows-api-openapi.yml
- filename: amazon-mediaconnect-gateway-instances-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Gateway Instances API
  slug: amazon-mediaconnect-gateway-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/openapi/amazon-mediaconnect-gateway-instances-api-openapi.yml
- filename: amazon-mediaconnect-gateways-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Gateways API
  slug: amazon-mediaconnect-gateways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/openapi/amazon-mediaconnect-gateways-api-openapi.yml
- filename: amazon-mediaconnect-offerings-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Offerings API
  slug: amazon-mediaconnect-offerings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/openapi/amazon-mediaconnect-offerings-api-openapi.yml
- filename: amazon-mediaconnect-reservations-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Reservations API
  slug: amazon-mediaconnect-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/openapi/amazon-mediaconnect-reservations-api-openapi.yml
- filename: amazon-mediaconnect-tags-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Tags API
  slug: amazon-mediaconnect-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/openapi/amazon-mediaconnect-tags-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- host: mediaconnect.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amazon Mediaconnect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon MediaConnect, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
slug: amazon-mediaconnect-domain-security
source_filename: amazon-mediaconnect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: mediaconnect.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/security/amazon-mediaconnect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
---
