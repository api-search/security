---
api_specs:
- filename: parlor-sh-openapi-generated.yml
  format: yaml
  label: Parlor.sh API
  slug: parlor-sh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parlor-sh/openapi/_ae-authored/parlor-sh-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: parlor.sh
  spf: true
hosts:
- cert_expires: Dec 22 05:14:31 2026 GMT
  host: parlor.sh
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Parlor.sh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parlor.sh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Parlor.sh
provider_slug: parlor-sh
slug: parlor-sh-domain-security
source_filename: parlor-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parlor.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 05:14:31 2026 GMT\n  hsts: false\ndomains:\n- domain: parlor.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/parlor-sh/security/parlor-sh-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Chat
- HTTP
- OpenAPI
- Privacy
---
