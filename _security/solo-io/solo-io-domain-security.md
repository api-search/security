---
api_specs:
- filename: solo-io-portal-server-openapi.yml
  format: yaml
  label: Gloo Portal Server API
  slug: portal-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-portal-server-openapi.yml
- filename: solo-io-portal-backend-openapi.yml
  format: yaml
  label: Gloo Portal Backend API
  slug: portal-backend
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-portal-backend-openapi.yml
- filename: solo-io-gloo-platform-portal-openapi.yml
  format: yaml
  label: Gloo Platform Portal API
  slug: gloo-platform-portal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-gloo-platform-portal-openapi.yml
- filename: solo-io-portal-idp-connect-openapi.yml
  format: yaml
  label: Gloo Portal IdP Connect API
  slug: portal-idp-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-portal-idp-connect-openapi.yml
- filename: solo-io-ai-gateway-guardrail-webhook-openapi.yml
  format: yaml
  label: AI Gateway Guardrail Webhook API
  slug: ai-guardrail-webhook
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-ai-gateway-guardrail-webhook-openapi.yml
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
- Model Context Protocol
- Developer Portal
- Cloud Native
- Open Source
---
