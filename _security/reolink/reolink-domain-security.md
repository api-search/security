---
api_specs:
- filename: reolink-camera-api-openapi.yml
  format: yaml
  label: Reolink Camera HTTP API
  slug: camera-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reolink/refs/heads/main/openapi/reolink-camera-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: reolink.com
  spf: true
hosts:
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: reolink.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 01:57:51 2026 GMT
  host: community.reolink.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reolink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reolink, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Reolink
provider_slug: reolink
slug: reolink-domain-security
source_filename: reolink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reolink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: community.reolink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 01:57:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: reolink.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reolink/refs/heads/main/security/reolink-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- IoT
- Security Cameras
- Surveillance
- Smart Home
- AI Detection
---
