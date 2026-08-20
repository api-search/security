---
api_specs:
- filename: shutterstock-audio-api-openapi.yml
  format: yaml
  label: Shutterstock audio API
  slug: shutterstock-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shutterstock/refs/heads/main/openapi/shutterstock-audio-api-openapi.yml
- filename: shutterstock-computer-vision-api-openapi.yml
  format: yaml
  label: Shutterstock computer_vision API
  slug: shutterstock-computer-vision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shutterstock/refs/heads/main/openapi/shutterstock-computer-vision-api-openapi.yml
- filename: shutterstock-contributors-api-openapi.yml
  format: yaml
  label: Shutterstock contributors API
  slug: shutterstock-contributors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shutterstock/refs/heads/main/openapi/shutterstock-contributors-api-openapi.yml
- filename: shutterstock-editorial-images-api-openapi.yml
  format: yaml
  label: Shutterstock editorial_images API
  slug: shutterstock-editorial-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shutterstock/refs/heads/main/openapi/shutterstock-editorial-images-api-openapi.yml
- filename: shutterstock-editorial-video-api-openapi.yml
  format: yaml
  label: Shutterstock editorial_video API
  slug: shutterstock-editorial-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shutterstock/refs/heads/main/openapi/shutterstock-editorial-video-api-openapi.yml
- filename: shutterstock-images-api-openapi.yml
  format: yaml
  label: Shutterstock images API
  slug: shutterstock-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shutterstock/refs/heads/main/openapi/shutterstock-images-api-openapi.yml
- filename: shutterstock-oauth-api-openapi.yml
  format: yaml
  label: Shutterstock oauth API
  slug: shutterstock-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shutterstock/refs/heads/main/openapi/shutterstock-oauth-api-openapi.yml
- filename: shutterstock-test-api-openapi.yml
  format: yaml
  label: Shutterstock test API
  slug: shutterstock-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shutterstock/refs/heads/main/openapi/shutterstock-test-api-openapi.yml
- filename: shutterstock-users-api-openapi.yml
  format: yaml
  label: Shutterstock users API
  slug: shutterstock-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shutterstock/refs/heads/main/openapi/shutterstock-users-api-openapi.yml
- filename: shutterstock-videos-api-openapi.yml
  format: yaml
  label: Shutterstock videos API
  slug: shutterstock-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shutterstock/refs/heads/main/openapi/shutterstock-videos-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shutterstock.com
  spf: true
hosts:
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: www.shutterstock.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: api.shutterstock.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Shutterstock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shutterstock, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Shutterstock
provider_slug: shutterstock
slug: shutterstock-domain-security
source_filename: shutterstock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shutterstock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: null\n- host: api.shutterstock.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: shutterstock.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shutterstock/refs/heads/main/security/shutterstock-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Image
- Media
- Photos
- Stock Images
- Videos
- Audio
- Licensing
- Creative Content
---
