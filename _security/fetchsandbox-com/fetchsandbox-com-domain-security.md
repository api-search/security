---
api_specs:
- filename: fetchsandbox-com-openapi-generated.yml
  format: yaml
  label: FetchSandbox API
  slug: fetchsandbox-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fetchsandbox-com/openapi/_ae-authored/fetchsandbox-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fetchsandbox.com
  spf: true
hosts:
- cert_expires: Feb  1 17:17:14 2027 GMT
  host: fetchsandbox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FetchSandbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FetchSandbox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FetchSandbox
provider_slug: fetchsandbox-com
slug: fetchsandbox-com-domain-security
source_filename: fetchsandbox-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fetchsandbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 17:17:14 2027 GMT\n  hsts: false\ndomains:\n- domain: fetchsandbox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/fetchsandbox-com/security/fetchsandbox-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Verification
- Sandbox
- Artificial Intelligence
- Testing
---
