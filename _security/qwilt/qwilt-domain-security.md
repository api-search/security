---
api_specs:
- filename: qwilt-media-delivery-openapi.yml
  format: yaml
  label: Qwilt CDN Media Delivery (Sites) API
  slug: qwilt-cdn-media-delivery-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qwilt/refs/heads/main/openapi/qwilt-media-delivery-openapi.yml
- filename: qwilt-certificate-manager-openapi.yml
  format: yaml
  label: Qwilt CDN Certificate Manager API
  slug: qwilt-cdn-certificate-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qwilt/refs/heads/main/openapi/qwilt-certificate-manager-openapi.yml
- filename: qwilt-origin-allow-list-openapi.yml
  format: yaml
  label: Qwilt CDN Origin Allow List API
  slug: qwilt-cdn-origin-allow-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qwilt/refs/heads/main/openapi/qwilt-origin-allow-list-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: qwilt.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: cqloud.com
  spf: false
hosts:
- cert_expires: Sep  5 16:46:20 2026 GMT
  host: www.qwilt.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: cert-manager.cqloud.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: media-sites.cqloud.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Qwilt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qwilt, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Qwilt
provider_slug: qwilt
slug: qwilt-domain-security
source_filename: qwilt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qwilt.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  5 16:46:20 2026 GMT\n  hsts: false\n- host: cert-manager.cqloud.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: null\n- host: media-sites.cqloud.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: qwilt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: cqloud.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qwilt/refs/heads/main/security/qwilt-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Media
- CDN
- Content Delivery Network
- Edge Computing
- Video Streaming
- Open Caching
- Media Delivery
- Certificates
- Infrastructure
---
