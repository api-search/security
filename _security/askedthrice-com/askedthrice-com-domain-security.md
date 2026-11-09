---
api_specs:
- filename: askedthrice-com-embeds-api-openapi.yml
  format: yaml
  label: Asked Thrice Embeds API
  slug: askedthrice-com-embeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/askedthrice-com/openapi/askedthrice-com-embeds-api-openapi.yml
- filename: askedthrice-com-scans-api-openapi.yml
  format: yaml
  label: Asked Thrice Scans API
  slug: askedthrice-com-scans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/askedthrice-com/openapi/askedthrice-com-scans-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: askedthrice.com
  spf: true
hosts:
- cert_expires: Nov 28 16:55:32 2026 GMT
  host: askedthrice.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Askedthrice Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Asked Thrice, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Asked Thrice
provider_slug: askedthrice-com
slug: askedthrice-com-domain-security
source_filename: askedthrice-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: askedthrice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 16:55:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: askedthrice.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/askedthrice-com/security/askedthrice-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Visibility
- Audit
- Generative AI
- Brand Analytics
---
