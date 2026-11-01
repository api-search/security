---
api_specs:
- filename: heretto-openapi-generated.yml
  format: yaml
  label: Heretto API
  slug: heretto-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heretto/openapi/_ae-authored/heretto-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "awstrust.com"
  - 0 issue "pki.goog"
  - 0 issue "amazontrust.com"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: heretto.com
  spf: true
hosts:
- cert_expires: Dec 12 08:35:51 2026 GMT
  host: heretto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Heretto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heretto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Heretto
provider_slug: heretto
slug: heretto-domain-security
source_filename: heretto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heretto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 08:35:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: heretto.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/heretto/security/heretto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- ContentOps
- Documentation
- Artificial Intelligence
- Collaboration
---
