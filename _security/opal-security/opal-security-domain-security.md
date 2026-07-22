---
api_specs:
- filename: opal-security-openapi.yaml
  format: yaml
  label: Opal API
  slug: opal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opal-security/refs/heads/main/openapi/opal-security-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: opal.dev
  spf: true
hosts:
- cert_expires: Oct  6 01:23:26 2026 GMT
  host: opal.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 02:19:08 2026 GMT
  host: api.opal.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opal Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opal Security, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Opal Security
provider_slug: opal-security
slug: opal-security-domain-security
source_filename: opal-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opal.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 01:23:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.opal.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 02:19:08 2026 GMT\n  hsts: false\ndomains:\n- domain: opal.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opal-security/refs/heads/main/security/opal-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Access Management
- Identity and Access Management
- Least Privilege
- Access Reviews
- Security
---
