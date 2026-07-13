---
api_specs:
- filename: snapchat-ads-api-openapi.yml
  format: yaml
  label: Snapchat Ads API
  slug: snapchat-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-ads-api-openapi.yml
- filename: snapchat-conversions-api-openapi.yml
  format: yaml
  label: Snapchat Conversions API
  slug: snapchat-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-conversions-api-openapi.yml
- filename: snapchat-login-kit-openapi.yml
  format: yaml
  label: Snapchat Login Kit API
  slug: snapchat-login-kit
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-login-kit-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: snap.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: snapchat.com
  spf: true
hosts:
- cert_expires: Sep 20 19:31:40 2026 GMT
  host: snap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 21:41:45 2026 GMT
  host: developers.snap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: adsapi.snapchat.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Snapchat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Snapchat, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Snapchat
provider_slug: snapchat
slug: snapchat-domain-security
source_filename: snapchat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 19:31:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.snap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 21:41:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: adsapi.snapchat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: snap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: snapchat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/security/snapchat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- AR
- Augmented Reality
- Marketing
- Messaging
- Social Media
---
