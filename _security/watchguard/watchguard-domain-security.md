---
api_specs:
- filename: watchguard-cloud-platform-openapi.yml
  format: yaml
  label: WatchGuard Cloud Platform API
  slug: watchguard-cloud-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/openapi/watchguard-cloud-platform-openapi.yml
- filename: watchguard-endpoint-security-openapi.yml
  format: yaml
  label: WatchGuard Endpoint Security Management API
  slug: watchguard-endpoint-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/openapi/watchguard-endpoint-security-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:itoperations@watchguard.com"
  - 0 issue "amazon.com"
  - 0 issue "cloudflare.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: watchguard.com
  spf: true
hosts:
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: www.watchguard.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: api.usa.cloud.watchguard.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.eu.cloud.watchguard.com
  https: false
kind: domain-security
layout: security
method: probed
name: Watchguard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WatchGuard, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: WatchGuard
provider_slug: watchguard
slug: watchguard-domain-security
source_filename: watchguard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.watchguard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.usa.cloud.watchguard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: null\n- host: api.eu.cloud.watchguard.com\n  https: false\ndomains:\n- domain: watchguard.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:itoperations@watchguard.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"cloudflare.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/security/watchguard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Security
- Endpoint Security
- Firewall
- MFA
- Network Security
- Zero Trust
---
