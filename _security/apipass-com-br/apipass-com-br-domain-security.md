---
api_specs:
- filename: apipass-com-br-openapi-generated.yml
  format: yaml
  label: Keila Santos API
  slug: apipass-com-br-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apipass-com-br/openapi/_ae-authored/apipass-com-br-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: apipass.com.br
  spf: true
hosts:
- cert_expires: Dec 12 13:05:18 2026 GMT
  host: apipass.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apipass Com Br Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keila Santos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Keila Santos
provider_slug: apipass-com-br
slug: apipass-com-br-domain-security
source_filename: apipass-com-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apipass.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 13:05:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apipass.com.br\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/apipass-com-br/security/apipass-com-br-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
---
