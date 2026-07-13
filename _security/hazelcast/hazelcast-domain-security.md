---
api_specs:
- filename: hazelcast-openapi.yml
  format: yaml
  label: Hazelcast REST API
  slug: hazelcast-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hazelcast/refs/heads/main/openapi/hazelcast-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hazelcast.com
  spf: true
hosts:
- cert_expires: Sep 16 23:16:17 2026 GMT
  host: hazelcast.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 13:59:10 2026 GMT
  host: docs.hazelcast.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hazelcast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hazelcast, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hazelcast
provider_slug: hazelcast
slug: hazelcast-domain-security
source_filename: hazelcast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hazelcast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:16:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.hazelcast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 13:59:10 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: hazelcast.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hazelcast/refs/heads/main/security/hazelcast-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Caching
- Distributed Computing
- In-Memory Computing
- Real-Time
- REST
---
