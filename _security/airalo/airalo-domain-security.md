---
api_specs:
- filename: airalo-partner-api-openapi.yml
  format: yaml
  label: Airalo Partner API
  slug: airalo-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airalo/refs/heads/main/openapi/airalo-partner-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: airalo.com
  spf: true
hosts:
- cert_expires: Nov  6 02:56:05 2026 GMT
  host: www.airalo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 02:56:05 2026 GMT
  host: partners.airalo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 00:01:53 2026 GMT
  host: developers.partners.airalo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Airalo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airalo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Airalo
provider_slug: airalo
slug: airalo-domain-security
source_filename: airalo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airalo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 02:56:05 2026 GMT\n  hsts: false\n- host: partners.airalo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 02:56:05 2026 GMT\n  hsts: false\n- host: developers.partners.airalo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 00:01:53 2026 GMT\n  hsts: false\ndomains:\n- domain: airalo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airalo/refs/heads/main/security/airalo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- eSIM
- Telecommunications
- Travel
- Connectivity
- Mobile Data
- Roaming
- Partner API
- Webhook
- Singapore
---
