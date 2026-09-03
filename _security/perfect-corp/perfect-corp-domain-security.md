---
api_specs:
- filename: perfect-corp-ai_abs_filter-openapi.yml
  format: yaml
  label: YouCam AI REST API
  slug: youcam-ai-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perfect-corp/refs/heads/main/openapi/perfect-corp-ai_abs_filter-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: perfectcorp.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: makeupar.com
  spf: true
hosts:
- cert_expires: Nov 26 12:46:01 2026 GMT
  host: docs.perfectcorp.com
  hsts: false
  https: true
  note: No Strict-Transport-Security header on the documentation host.
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: yce-api-01.makeupar.com
  hsts: true
  hsts_header: max-age=31536000; includeSubdomains;
  https: true
  note: The automated probe read null because the API host answers its root with a JSON 404; the HSTS header IS returned on an authenticated-route response (observed on a 401 from GET /s2s/v2.0/credit/feature-cost, 2026-09-02).
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Perfect Corp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Perfect Corp, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Perfect Corp
provider_slug: perfect-corp
slug: perfect-corp-domain-security
source_filename: perfect-corp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.perfectcorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 12:46:01 2026 GMT\n  hsts: false\n  note: No Strict-Transport-Security header on the documentation host.\n- host: yce-api-01.makeupar.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_header: max-age=31536000; includeSubdomains;\n  note: The automated probe read null because the API host answers its root with a JSON 404; the HSTS header IS\n    returned on an authenticated-route response (observed on a 401 from GET /s2s/v2.0/credit/feature-cost, 2026-09-02).\ndomains:\n- domain: perfectcorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: makeupar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nobserved_response_headers:\n  host: yce-api-01.makeupar.com\n\
  \  sample: GET /s2s/v2.0/credit/feature-cost with an invalid bearer token -> HTTP 401\n  headers:\n  - 'server: nginx'\n  - 'x-request-id: <snowflake id>'\n  - 'x-frame-options: sameorigin'\n  - 'strict-transport-security: max-age=31536000; includeSubdomains;'\n  - 'vary: Origin'\n  absent:\n  - RateLimit-*\n  - X-RateLimit-*\n  - Retry-After\n  - Content-Security-Policy\n  - X-Content-Type-Options\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perfect-corp/refs/heads/main/security/perfect-corp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- beauty
- skincare
- cosmetics
- fashion
- apparel
- jewelry
- watches
- hair
- virtual-try-on
- image-editing
- generative-ai
- computer-vision
- AR
- visual-commerce
- ai
- machine-learning
- video-generation
- skin-analysis
- mcp
- agents
- photo-editing
- beauty-tech
- retail
- ar-try-on
---
