---
api_specs:
- filename: ironfang-account-api-openapi.yml
  format: yaml
  label: Ironfang Account API
  slug: ironfang-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironfang/refs/heads/main/openapi/ironfang-account-api-openapi.yml
- filename: ironfang-batches-api-openapi.yml
  format: yaml
  label: Ironfang Batches API
  slug: ironfang-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironfang/refs/heads/main/openapi/ironfang-batches-api-openapi.yml
- filename: ironfang-destinations-api-openapi.yml
  format: yaml
  label: Ironfang Destinations API
  slug: ironfang-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironfang/refs/heads/main/openapi/ironfang-destinations-api-openapi.yml
- filename: ironfang-jobs-api-openapi.yml
  format: yaml
  label: Ironfang Jobs API
  slug: ironfang-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironfang/refs/heads/main/openapi/ironfang-jobs-api-openapi.yml
- filename: ironfang-render-api-openapi.yml
  format: yaml
  label: Ironfang Render API
  slug: ironfang-render-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironfang/refs/heads/main/openapi/ironfang-render-api-openapi.yml
- filename: ironfang-signed-urls-api-openapi.yml
  format: yaml
  label: Ironfang Signed URLs API
  slug: ironfang-signed-urls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironfang/refs/heads/main/openapi/ironfang-signed-urls-api-openapi.yml
- filename: ironfang-templates-api-openapi.yml
  format: yaml
  label: Ironfang Templates API
  slug: ironfang-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironfang/refs/heads/main/openapi/ironfang-templates-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ironfang.uk
  spf: true
hosts:
- cert_expires: Oct 20 08:01:32 2026 GMT
  host: ironfang.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 08:01:32 2026 GMT
  host: api.ironfang.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Ironfang Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ironfang, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ironfang
provider_slug: ironfang
slug: ironfang-domain-security
source_filename: ironfang-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ironfang.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 08:01:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ironfang.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 08:01:32 2026 GMT\n  hsts: null\ndomains:\n- domain: ironfang.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ironfang/refs/heads/main/security/ironfang-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Developer Tools
- screenshot-api
- website screenshot
- HTML to PDF
- PDF API
- Image API
- OG Image API
- QR Code API
- Website-to-Video
- Rendering Infrastructure
- MCP
- UK-hosted
---
