---
api_specs:
- filename: vertex-openapi-generated.yml
  format: yaml
  label: Vertex API
  slug: vertex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vertex/refs/heads/main/openapi/_ae-authored/vertex-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vertexinc.com
  spf: true
hosts:
- cert_expires: Dec 12 15:20:31 2026 GMT
  host: www.vertexinc.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vertex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vertex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vertex
provider_slug: vertex
slug: vertex-domain-security
source_filename: vertex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vertexinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 15:20:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: vertexinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vertex/refs/heads/main/security/vertex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Tax
- Compliance
- API
- Automation
---
