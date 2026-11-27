---
api_specs:
- filename: tandem-ac-openapi-generated.yml
  format: yaml
  label: Tandem API
  slug: tandem-ac-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tandem-ac/openapi/_ae-authored/tandem-ac-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: tandem.ac
  spf: false
hosts:
- cert_expires: Feb 15 23:49:57 2027 GMT
  host: tandem.ac
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tandem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tandem, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Tandem
provider_slug: tandem-ac
slug: tandem-ac-domain-security
source_filename: tandem-ac-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tandem.ac\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 23:49:57 2027 GMT\n  hsts: false\ndomains:\n- domain: tandem.ac\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tandem-ac/security/tandem-ac-domain-security.yml
summary_line: TLSv1.3
tags:
- AI Governance
- Runtime
- Audit
- Enterprise AI
- Tool Access
---
