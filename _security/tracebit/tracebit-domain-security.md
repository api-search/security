---
api_specs:
- filename: tracebit-community-openapi-original.json
  format: json
  label: Tracebit API (Community Edition)
  slug: tracebit-api-community-edition
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tracebit/refs/heads/main/openapi/tracebit-community-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tracebit.com
  spf: true
hosts:
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: tracebit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tracebit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tracebit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tracebit
provider_slug: tracebit
slug: tracebit-domain-security
source_filename: tracebit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tracebit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tracebit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tracebit/refs/heads/main/security/tracebit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cloud Saas
- Security
- Deception
- Canary Tokens
- Threat Detection
- Cloud Security
- Incident Response
---
