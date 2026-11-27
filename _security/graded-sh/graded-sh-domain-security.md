---
api_specs:
- filename: graded-sh-services-api-openapi.yml
  format: yaml
  label: Graded Services API
  slug: graded-sh-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/graded-sh/openapi/graded-sh-services-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: graded.sh
  spf: true
hosts:
- cert_expires: Dec 21 00:01:03 2026 GMT
  host: graded.sh
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Graded Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Graded, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Graded
provider_slug: graded-sh
slug: graded-sh-domain-security
source_filename: graded-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: graded.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 00:01:03 2026 GMT\n  hsts: false\ndomains:\n- domain: graded.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/graded-sh/security/graded-sh-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Payments
- Gateways
- API-Index
- AgentEconomy
---
