---
api_specs:
- filename: stackrox-openapi.yml
  format: yaml
  label: StackRox API
  slug: stackrox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackrox/refs/heads/main/openapi/stackrox-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: stackrox.io
  spf: true
hosts:
- cert_expires: Sep 23 20:11:14 2026 GMT
  host: www.stackrox.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stackrox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StackRox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: StackRox
provider_slug: stackrox
slug: stackrox-domain-security
source_filename: stackrox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stackrox.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 20:11:14 2026 GMT\n  hsts: false\ndomains:\n- domain: stackrox.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stackrox/refs/heads/main/security/stackrox-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Compliance
- Container Security
- Kubernetes
- Open Source
- Runtime Protection
- Security
---
