---
api_specs:
- filename: linkpeek-favicon-api-openapi.yml
  format: yaml
  label: LinkPeek Favicon API
  slug: linkpeek-favicon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkpeek/refs/heads/main/openapi/linkpeek-favicon-api-openapi.yml
- filename: linkpeek-link-preview-api-openapi.yml
  format: yaml
  label: LinkPeek Link Preview API
  slug: linkpeek-link-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkpeek/refs/heads/main/openapi/linkpeek-link-preview-api-openapi.yml
- filename: linkpeek-meta-tags-api-openapi.yml
  format: yaml
  label: LinkPeek Meta Tags API
  slug: linkpeek-meta-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkpeek/refs/heads/main/openapi/linkpeek-meta-tags-api-openapi.yml
- filename: linkpeek-qr-code-api-openapi.yml
  format: yaml
  label: LinkPeek QR Code API
  slug: linkpeek-qr-code-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkpeek/refs/heads/main/openapi/linkpeek-qr-code-api-openapi.yml
- filename: linkpeek-system-api-openapi.yml
  format: yaml
  label: LinkPeek System API
  slug: linkpeek-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkpeek/refs/heads/main/openapi/linkpeek-system-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: linkpeek.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sslip.io
  spf: true
hosts:
- cert_expires: Sep 18 02:21:43 2026 GMT
  host: linkpeek.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 19:04:43 2026 GMT
  host: 147.15.103.217.sslip.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linkpeek Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LinkPeek, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: LinkPeek
provider_slug: linkpeek
slug: linkpeek-domain-security
source_filename: linkpeek-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linkpeek.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 02:21:43 2026 GMT\n  hsts: false\n- host: 147.15.103.217.sslip.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 19:04:43 2026 GMT\n  hsts: false\ndomains:\n- domain: linkpeek.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: sslip.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linkpeek/refs/heads/main/security/linkpeek-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Screenshots
- webpage-capture
- website-thumbnails
- Image-Generation
- Rendering
- web-scraping-adjacent
- Developer Tools
- Software-as-a-Service
- rest-image-api
- Utility API
- URL Metadata
- Link Preview
- OpenGraph
- QR Code Generation
- DNS
- WHOIS
- SSL
- Web Security Scanning
- IP Geolocation
- Data Conversion
- LLM-Compatible API
- API Utilities
- dns-whois
- openai-compatible-llm
---
