---
api_specs:
- filename: truth-systems-gateway-openapi-original.json
  format: json
  label: Truth Systems Gateway API
  slug: truth-systems-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truth-systems/refs/heads/main/openapi/truth-systems-gateway-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: truthsystems.ai
  spf: true
hosts:
- cert_expires: Oct 17 16:21:09 2026 GMT
  host: www.truthsystems.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 15:01:54 2026 GMT
  host: docs.truthsystems.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Truth Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Truth Systems, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Truth Systems
provider_slug: truth-systems
slug: truth-systems-domain-security
source_filename: truth-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.truthsystems.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 16:21:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.truthsystems.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 15:01:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: truthsystems.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truth-systems/refs/heads/main/security/truth-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Governance
- Hallucination Detection
- Fact Checking
- Compliance
- Legal
---
