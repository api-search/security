---
api_specs:
- filename: warner-bros-discovery-content-partner-openapi.yml
  format: yaml
  label: Warner Bros. Discovery Content Partner API
  slug: wbd-content-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warner-bros-discovery/refs/heads/main/openapi/warner-bros-discovery-content-partner-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wbd.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: warnermedia.com
  spf: true
hosts:
- cert_expires: Aug 10 17:31:01 2026 GMT
  host: www.wbd.com
  hsts: true
  hsts_max_age: 60
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: partnerhub.warnermedia.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 17:02:44 2026 GMT
  host: www.max.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Warner Bros Discovery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Warner Bros. Discovery, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Warner Bros. Discovery
provider_slug: warner-bros-discovery
slug: warner-bros-discovery-domain-security
source_filename: warner-bros-discovery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wbd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 17:31:01 2026 GMT\n  hsts: true\n  hsts_max_age: 60\n- host: partnerhub.warnermedia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: false\n- host: www.max.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 17:02:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wbd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: warnermedia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/warner-bros-discovery/refs/heads/main/security/warner-bros-discovery-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Entertainment
- Media
- Streaming
- Content
- Television
- Film
---
