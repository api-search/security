---
api_specs:
- filename: miele-openapi-generated.yml
  format: yaml
  label: Miele API
  slug: miele-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/miele/openapi/_ae-authored/miele-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: miele.com
  spf: true
hosts:
- cert_expires: Mar 20 23:59:59 2027 GMT
  host: miele.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Miele Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Miele, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Miele
provider_slug: miele
slug: miele-domain-security
source_filename: miele-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: miele.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: miele.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/miele/security/miele-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Appliances
- Home
- Technology
- German
---
