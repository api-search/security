---
api_specs:
- filename: spot-administration-api-openapi.yml
  format: yaml
  label: Spot Administration API
  slug: administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-administration-api-openapi.yml
- filename: spot-elastigroup-api-openapi.yml
  format: yaml
  label: Spot Elastigroup API
  slug: elastigroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-elastigroup-api-openapi.yml
- filename: spot-ocean-api-openapi.yml
  format: yaml
  label: Spot Ocean API
  slug: ocean-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-ocean-api-openapi.yml
- filename: spot-eco-api-openapi.yml
  format: yaml
  label: Spot Eco API
  slug: eco-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-eco-api-openapi.yml
- filename: spot-billing-engine-api-openapi.yml
  format: yaml
  label: Spot Billing Engine API
  slug: billing-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-billing-engine-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spot.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spotinst.io
  spf: false
hosts:
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: docs.spot.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: api.spotinst.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Spot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spot, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Spot
provider_slug: spot
slug: spot-domain-security
source_filename: spot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.spot.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.spotinst.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: spot.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: spotinst.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/security/spot-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Autoscaling
- Cloud Infrastructure
- Containers
- Cost Optimization
- FinOps
- Kubernetes
- Spot Instances
---
