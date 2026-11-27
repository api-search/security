---
api_specs:
- filename: 1099-pro-openapi-generated.yml
  format: yaml
  label: Sovos Compliance, LLC API
  slug: 1099-pro-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/1099-pro/openapi/_ae-authored/1099-pro-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 1099pro.com
  spf: true
hosts:
- cert_expires: Dec 30 09:58:14 2026 GMT
  host: 1099pro.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sovos Compliance, LLC Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sovos Compliance, LLC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sovos Compliance, LLC
provider_slug: 1099-pro
slug: 1099-pro-domain-security
source_filename: 1099-pro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 1099pro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 09:58:14 2026 GMT\n  hsts: false\ndomains:\n- domain: 1099pro.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/1099-pro/security/1099-pro-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Tax Software
- Efiling
- Compliance
- Software-as-a-Service
- Financial Services
---
