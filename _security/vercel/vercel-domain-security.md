---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Vercel REST API
  slug: vercel-rest-api
  spec_type: OpenAPI
  url: https://openapi.vercel.sh/
- filename: vercel-ai-gateway-openapi.yml
  format: yaml
  label: Vercel AI Gateway API
  slug: vercel-ai-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vercel/refs/heads/main/openapi/vercel-ai-gateway-openapi.yml
- filename: vercel-webhooks-asyncapi.yml
  format: yaml
  label: Vercel Webhooks
  slug: vercel-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/vercel/refs/heads/main/asyncapi/vercel-webhooks-asyncapi.yml
- filename: vercel-v0-platform-openapi.yml
  format: yaml
  label: V0 Platform API
  slug: v0-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vercel/refs/heads/main/openapi/vercel-v0-platform-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vercel.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: v0.dev
  spf: false
hosts:
- cert_expires: Aug 21 08:55:49 2026 GMT
  host: vercel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 15:28:19 2026 GMT
  host: v0.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 05:08:17 2026 GMT
  host: ai-gateway.vercel.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vercel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vercel, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vercel
provider_slug: vercel
slug: vercel-domain-security
source_filename: vercel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vercel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 08:55:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: v0.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 15:28:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: ai-gateway.vercel.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 05:08:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: vercel.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: v0.dev\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vercel/refs/heads/main/security/vercel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Gateways
- Gateways
- Observability
- Webhooks
---
