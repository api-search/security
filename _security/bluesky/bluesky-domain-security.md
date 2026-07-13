---
api_specs:
- filename: bluesky-openapi.yml
  format: yaml
  label: Bluesky API
  slug: bluesky-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluesky/refs/heads/main/openapi/bluesky-openapi.yml
- filename: bluesky-asyncapi.yml
  format: yaml
  label: Bluesky Jetstream
  slug: bluesky-jetstream
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluesky/refs/heads/main/asyncapi/bluesky-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bsky.app
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bsky.social
  spf: false
hosts:
- cert_expires: Aug 24 02:04:29 2026 GMT
  host: docs.bsky.app
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: bsky.social
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 21:05:26 2026 GMT
  host: public.api.bsky.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bluesky Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bluesky, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bluesky
provider_slug: bluesky
slug: bluesky-domain-security
source_filename: bluesky-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.bsky.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 02:04:29 2026 GMT\n  hsts: false\n- host: bsky.social\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: false\n- host: public.api.bsky.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 21:05:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bsky.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: bsky.social\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluesky/refs/heads/main/security/bluesky-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- At-Protocol
- Decentralized
- Federated
- Open-Source
- Social Networks
- Social-Media
---
