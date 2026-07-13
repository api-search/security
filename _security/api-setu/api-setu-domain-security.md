---
description: ''
domains:
- caa:
  - 0 issue "emsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: apisetu.gov.in
  spf: true
hosts:
- cert_expires: Aug 16 03:23:36 2026 GMT
  host: www.apisetu.gov.in
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Api Setu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for API Setu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: API Setu
provider_slug: api-setu
slug: api-setu-domain-security
source_filename: api-setu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apisetu.gov.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 03:23:36 2026 GMT\n  hsts: null\ndomains:\n- domain: apisetu.gov.in\n  dnssec: false\n  caa:\n  - 0 issue \"emsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-setu/refs/heads/main/security/api-setu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Open Data
- Public APIs
---
