---
api_specs:
- filename: platform.sh-rest-api-openapi.json
  format: json
  label: Platform.sh REST API
  slug: platform.sh-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/platform.sh/refs/heads/main/openapi/platform.sh-rest-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: upsun.com
  spf: true
- caa:
  - pki.goog
  - sectigo.com
  - amazontrust.com
  - digicert.com
  - letsencrypt.org
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: platform.sh
  note: Probed 2026-08-26 via dig/openssl. No DS record published, so DNSSEC is not enabled on platform.sh.
  spf: true
hosts:
- cert_expires: Nov  2 03:17:46 2026 GMT
  host: upsun.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 13:16:30 2026 GMT
  host: developer.upsun.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 19:07:59 2026 GMT
  host: api.upsun.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 11:12:08 2026 GMT
  host: platform.sh
  hsts: true
  hsts_max_age: 31557600
  https: true
  note: Legacy brand host. Serves /.well-known/security.txt directly (200); / 301s to upsun.com.
  tls_version: TLSv1.3
- cert_expires: Nov 12 07:48:36 2026 GMT
  host: auth.api.platform.sh
  hsts: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: OAuth 2.0 authorization server for the REST API; still on the platform.sh domain after the Upsun rebrand.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Platform.Sh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Platform.sh, probed live across 5 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 5 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Platform.sh
provider_slug: platform.sh
slug: platform.sh-domain-security
source_filename: platform.sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts, plus manual dig/openssl probes of platform.sh and\n  auth.api.platform.sh\nhosts:\n- host: upsun.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 03:17:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developer.upsun.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 13:16:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.upsun.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 19:07:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: platform.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 11:12:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n  note: Legacy brand host. Serves /.well-known/security.txt directly (200); / 301s to upsun.com.\n- host: auth.api.platform.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 07:48:36 2026 GMT\n  hsts: true\n  hsts_max_age:\
  \ 31536000\n  hsts_preload: true\n  note: OAuth 2.0 authorization server for the REST API; still on the platform.sh domain after the Upsun rebrand.\ndomains:\n- domain: upsun.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: platform.sh\n  dnssec: false\n  caa:\n  - pki.goog\n  - sectigo.com\n  - amazontrust.com\n  - digicert.com\n  - letsencrypt.org\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  note: Probed 2026-08-26 via dig/openssl. No DS record published, so DNSSEC is not enabled on platform.sh.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/platform.sh/refs/heads/main/security/platform.sh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Platform as a Service
- Cloud Hosting
- Application Hosting
- Deployment
- DevOps
- Continuous Deployment
- Containers
- Managed Services
- Developer Tools
- Infrastructure
- Multicloud
- Web Hosting
---
