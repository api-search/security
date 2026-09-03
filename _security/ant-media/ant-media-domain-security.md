---
api_specs:
- filename: ant-media-broadcasts-api-openapi.yml
  format: yaml
  label: Ant Media Broadcasts API
  slug: ant-media-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ant-media/refs/heads/main/openapi/ant-media-broadcasts-api-openapi.yml
- filename: ant-media-filters-api-openapi.yml
  format: yaml
  label: Ant Media Filters API
  slug: ant-media-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ant-media/refs/heads/main/openapi/ant-media-filters-api-openapi.yml
- filename: ant-media-push-notification-api-openapi.yml
  format: yaml
  label: Ant Media Push Notification API
  slug: ant-media-push-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ant-media/refs/heads/main/openapi/ant-media-push-notification-api-openapi.yml
- filename: ant-media-version-api-openapi.yml
  format: yaml
  label: Ant Media Version API
  slug: ant-media-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ant-media/refs/heads/main/openapi/ant-media-version-api-openapi.yml
- filename: ant-media-vods-api-openapi.yml
  format: yaml
  label: Ant Media Vods API
  slug: ant-media-vods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ant-media/refs/heads/main/openapi/ant-media-vods-api-openapi.yml
- filename: ant-media-management-api-openapi.yml
  format: yaml
  label: Ant Media Management API
  slug: ant-media-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ant-media/refs/heads/main/openapi/ant-media-management-api-openapi.yml
- filename: ant-media-cluster-api-openapi.yml
  format: yaml
  label: Ant Media Cluster API
  slug: ant-media-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ant-media/refs/heads/main/openapi/ant-media-cluster-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: antmedia.io
  spf: true
hosts:
- cert_expires: Nov 19 07:42:49 2026 GMT
  host: antmedia.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 02:01:40 2026 GMT
  host: test.antmedia.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ant Media Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ant Media, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Ant Media
provider_slug: ant-media
slug: ant-media-domain-security
source_filename: ant-media-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: antmedia.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 07:42:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: test.antmedia.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 02:01:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: antmedia.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ant-media/refs/heads/main/security/ant-media-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Broadcasting
- Live Streaming
- Media
- Streaming
- Video
- WebRTC
---
