---
api_specs:
- filename: a2-biotherapeutics-wp-rest-openapi.yml
  format: yaml
  label: A2 Biotherapeutics WordPress REST API
  slug: a2-biotherapeutics-wordpress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/a2-biotherapeutics/refs/heads/main/openapi/a2-biotherapeutics-wp-rest-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: a2bio.com
  spf: true
hosts:
- cert_expires: Oct  6 04:12:11 2026 GMT
  host: www.a2bio.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: A2 Biotherapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for A2 Biotherapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: A2 Biotherapeutics
provider_slug: a2-biotherapeutics
slug: a2-biotherapeutics-domain-security
source_filename: a2-biotherapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.a2bio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 04:12:11 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: a2bio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/a2-biotherapeutics/refs/heads/main/security/a2-biotherapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Life Sciences
- Cell Therapy
- Immuno-Oncology
- Oncology
- Pharmaceuticals
- Clinical Trials
- Healthcare
- Model Context Protocol
- WordPress
---
