---
api_specs:
- filename: ditto-live-api-keys-api-openapi.yml
  format: yaml
  label: Ditto API Keys API
  slug: ditto-live-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ditto-live/refs/heads/main/openapi/ditto-live-api-keys-api-openapi.yml
- filename: ditto-live-apps-api-openapi.yml
  format: yaml
  label: Ditto Apps API
  slug: ditto-live-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ditto-live/refs/heads/main/openapi/ditto-live-apps-api-openapi.yml
- filename: ditto-live-bigpeerreplication-api-openapi.yml
  format: yaml
  label: Ditto BigPeerReplication API
  slug: ditto-live-bigpeerreplication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ditto-live/refs/heads/main/openapi/ditto-live-bigpeerreplication-api-openapi.yml
- filename: ditto-live-data-bridge-api-openapi.yml
  format: yaml
  label: Ditto Data Bridge API
  slug: ditto-live-data-bridge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ditto-live/refs/heads/main/openapi/ditto-live-data-bridge-api-openapi.yml
- filename: ditto-live-store-api-openapi.yml
  format: yaml
  label: Ditto Store API
  slug: ditto-live-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ditto-live/refs/heads/main/openapi/ditto-live-store-api-openapi.yml
- filename: ditto-live-sync-api-openapi.yml
  format: yaml
  label: Ditto Sync API
  slug: ditto-live-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ditto-live/refs/heads/main/openapi/ditto-live-sync-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ditto.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ditto.live
  spf: true
hosts:
- cert_expires: Sep 12 18:31:05 2026 GMT
  host: www.ditto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: portal.ditto.live
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 17:13:53 2026 GMT
  host: docs.ditto.live
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ditto Live Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ditto, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ditto
provider_slug: ditto-live
slug: ditto-live-domain-security
source_filename: ditto-live-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ditto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 18:31:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal.ditto.live\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: false\n- host: docs.ditto.live\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 17:13:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ditto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ditto.live\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ditto-live/refs/heads/main/security/ditto-live-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Developer Tools
- Database
- Synchronization
- Peer-to-Peer
- Edge Computing
- Offline-First
- Mobile
---
