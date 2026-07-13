---
api_specs:
- filename: neuvector-openapi-original.yaml
  format: yaml
  label: NeuVector
  slug: neuvector
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neuvector/refs/heads/main/openapi/neuvector-openapi-original.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: neuvector.com
  spf: true
hosts:
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: neuvector.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 17:02:20 2026 GMT
  host: open-docs.neuvector.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neuvector Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NeuVector, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: NeuVector
provider_slug: neuvector
slug: neuvector-domain-security
source_filename: neuvector-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: neuvector.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: open-docs.neuvector.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 17:02:20 2026 GMT\n  hsts: false\ndomains:\n- domain: neuvector.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neuvector/refs/heads/main/security/neuvector-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Compliance
- Containers
- Kubernetes
- Open Source
- Runtime Protection
- Security
- Vulnerability Scanning
---
