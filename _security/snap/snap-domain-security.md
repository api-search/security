---
api_specs:
- filename: snap-conversion-api-openapi.yml
  format: yaml
  label: Snap Conversion API
  slug: snap-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snap/refs/heads/main/openapi/snap-conversion-api-openapi.yml
- filename: snap-events-api-openapi.yml
  format: yaml
  label: Snap Events API
  slug: snap-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snap/refs/heads/main/openapi/snap-events-api-openapi.yml
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
- cert_expires: Nov  7 14:58:31 2026 GMT
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
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: tr.snapchat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Snap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Snap, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Snap
provider_slug: snap
slug: snap-domain-security
source_filename: snap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.snap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 14:58:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: adsapi.snapchat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: null\n- host: tr.snapchat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: snap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: snapchat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snap/refs/heads/main/security/snap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- Marketing
- Social-Media
- Augmented Reality
- Camera
- Authentication
- Identity
- Conversions
- Attribution
- SDK
---
