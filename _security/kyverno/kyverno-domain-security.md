---
api_specs:
- filename: kyverno-policy-reporter-openapi.yml
  format: yaml
  label: Kyverno Policy Reporter API
  slug: kyverno-policy-reporter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kyverno/refs/heads/main/openapi/kyverno-policy-reporter-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kyverno.io
  spf: false
hosts:
- cert_expires: Aug 26 08:45:52 2026 GMT
  host: kyverno.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kyverno Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kyverno, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Kyverno
provider_slug: kyverno
slug: kyverno-domain-security
source_filename: kyverno-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kyverno.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 08:45:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kyverno.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kyverno/refs/heads/main/security/kyverno-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cloud Native
- Governance
- Kubernetes
- Policy Management
- Security
---
