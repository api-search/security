---
api_specs:
- filename: slb-openapi-generated.yml
  format: yaml
  label: SLB API
  slug: slb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/slb/openapi/_ae-authored/slb-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:pki-admin-manager@slb.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: slb.com
  spf: true
hosts:
- cert_expires: Jan  1 15:07:14 2027 GMT
  host: developer.slb.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SLB Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SLB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SLB
provider_slug: slb
slug: slb-domain-security
source_filename: slb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.slb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 15:07:14 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: slb.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:pki-admin-manager@slb.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/slb/security/slb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Oilfield Services
- Engineering
---
