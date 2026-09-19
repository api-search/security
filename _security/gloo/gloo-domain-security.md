---
api_specs:
- filename: gloo-api-products-api-openapi.yml
  format: yaml
  label: Gloo API Products API
  slug: gloo-api-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gloo/refs/heads/main/openapi/gloo-api-products-api-openapi.yml
- filename: gloo-applications-api-openapi.yml
  format: yaml
  label: Gloo Applications API
  slug: gloo-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gloo/refs/heads/main/openapi/gloo-applications-api-openapi.yml
- filename: gloo-me-api-openapi.yml
  format: yaml
  label: Gloo Me API
  slug: gloo-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gloo/refs/heads/main/openapi/gloo-me-api-openapi.yml
- filename: gloo-subscriptions-api-openapi.yml
  format: yaml
  label: Gloo Subscriptions API
  slug: gloo-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gloo/refs/heads/main/openapi/gloo-subscriptions-api-openapi.yml
- filename: gloo-teams-api-openapi.yml
  format: yaml
  label: Gloo Teams API
  slug: gloo-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gloo/refs/heads/main/openapi/gloo-teams-api-openapi.yml
- filename: gloo-user-api-openapi.yml
  format: yaml
  label: Gloo User API
  slug: gloo-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gloo/refs/heads/main/openapi/gloo-user-api-openapi.yml
- filename: gloo-webhooks-api-openapi.yml
  format: yaml
  label: Gloo Webhooks API
  slug: gloo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gloo/refs/heads/main/openapi/gloo-webhooks-api-openapi.yml
- filename: gloo-apis-api-openapi.yml
  format: yaml
  label: Gloo AP Is API
  slug: gloo-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gloo/refs/heads/main/openapi/gloo-apis-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: solo.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: gloo-platform-portal.com
  spf: false
hosts:
- cert_expires: Oct 14 07:07:34 2026 GMT
  host: www.solo.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 15:32:53 2026 GMT
  host: docs.solo.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.gloo-platform-portal.com
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Gloo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gloo, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gloo
provider_slug: gloo
slug: gloo-domain-security
source_filename: gloo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.solo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 07:07:34 2026 GMT\n  hsts: false\n- host: docs.solo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 15:32:53 2026 GMT\n  hsts: false\n- host: api.gloo-platform-portal.com\n  https: false\ndomains:\n- domain: solo.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: gloo-platform-portal.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gloo/refs/heads/main/security/gloo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API Gateway
- Cloud-Native
- Developer Portal
- Envoy
- Istio
- Kubernetes
- Kubernetes Gateway API
- Open-Source
- Service Mesh
---
