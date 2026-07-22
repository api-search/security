---
api_specs:
- filename: supernormal-openapi-original.json
  format: json
  label: Supernormal API
  slug: supernormal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supernormal/refs/heads/main/openapi/supernormal-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: supernormal.com
  spf: true
hosts:
- cert_expires: Oct 17 10:07:42 2026 GMT
  host: supernormal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 06:30:26 2026 GMT
  host: docs.supernormal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 08:03:32 2026 GMT
  host: api.supernormal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Supernormal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for supernormal, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: supernormal
provider_slug: supernormal
slug: supernormal-domain-security
source_filename: supernormal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: supernormal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 10:07:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.supernormal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 06:30:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.supernormal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 08:03:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: supernormal.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/supernormal/refs/heads/main/security/supernormal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Meetings
- Meeting Notes
- Transcription
- AI Agents
- Voice Agents
- Productivity
- Collaboration
- Model Context Protocol
- REST API
---
