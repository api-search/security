---
api_specs:
- filename: solo-io-api-keys-api-openapi.yml
  format: yaml
  label: Solo.io API Keys API
  slug: solo-io-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-api-keys-api-openapi.yml
- filename: solo-io-api-products-api-openapi.yml
  format: yaml
  label: Solo.io API Products API
  slug: solo-io-api-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-api-products-api-openapi.yml
- filename: solo-io-apis-api-openapi.yml
  format: yaml
  label: Solo.io AP Is API
  slug: solo-io-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-apis-api-openapi.yml
- filename: solo-io-applications-api-openapi.yml
  format: yaml
  label: Solo.io Applications API
  slug: solo-io-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-applications-api-openapi.yml
- filename: solo-io-apps-api-openapi.yml
  format: yaml
  label: Solo.io Apps API
  slug: solo-io-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-apps-api-openapi.yml
- filename: solo-io-auth-api-openapi.yml
  format: yaml
  label: Solo.io Auth API
  slug: solo-io-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-auth-api-openapi.yml
- filename: solo-io-health-api-openapi.yml
  format: yaml
  label: Solo.io Health API
  slug: solo-io-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-health-api-openapi.yml
- filename: solo-io-me-api-openapi.yml
  format: yaml
  label: Solo.io Me API
  slug: solo-io-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-me-api-openapi.yml
- filename: solo-io-metadata-api-openapi.yml
  format: yaml
  label: Solo.io Metadata API
  slug: solo-io-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-metadata-api-openapi.yml
- filename: solo-io-oauth-credentials-api-openapi.yml
  format: yaml
  label: Solo.io OAUTH Credentials API
  slug: solo-io-oauth-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-oauth-credentials-api-openapi.yml
- filename: solo-io-subscriptions-api-openapi.yml
  format: yaml
  label: Solo.io Subscriptions API
  slug: solo-io-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-subscriptions-api-openapi.yml
- filename: solo-io-teams-api-openapi.yml
  format: yaml
  label: Solo.io Teams API
  slug: solo-io-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-teams-api-openapi.yml
- filename: solo-io-user-api-openapi.yml
  format: yaml
  label: Solo.io User API
  slug: solo-io-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-user-api-openapi.yml
- filename: solo-io-users-api-openapi.yml
  format: yaml
  label: Solo.io Users API
  slug: solo-io-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-users-api-openapi.yml
- filename: solo-io-webhooks-api-openapi.yml
  format: yaml
  label: Solo.io Webhooks API
  slug: solo-io-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
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
- cert_expires: Oct  3 16:29:55 2026 GMT
  host: docs.solo.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.gloo-platform-portal.com
  https: false
kind: domain-security
layout: security
method: probed
name: Solo Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Solo.io, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Solo.io
provider_slug: solo-io
slug: solo-io-domain-security
source_filename: solo-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.solo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 07:07:34 2026 GMT\n  hsts: false\n- host: docs.solo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 16:29:55 2026 GMT\n  hsts: false\n- host: api.gloo-platform-portal.com\n  https: false\ndomains:\n- domain: solo.io\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: gloo-platform-portal.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/security/solo-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- API Gateway
- Service Mesh
- Kubernetes
- Istio
- Envoy
- AI Gateway
- Agentic AI
- MCP
- Developer Portal
- Cloud-Native
- Open-Source
---
