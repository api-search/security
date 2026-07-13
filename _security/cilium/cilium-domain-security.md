---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Cilium API
  slug: cilium-api
  spec_type: OpenAPI
  url: https://github.com/cilium/cilium/blob/main/api/v1/openapi.yaml
- filename: cilium-hubble-asyncapi.yml
  format: yaml
  label: Hubble API
  slug: hubble-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cilium/refs/heads/main/asyncapi/cilium-hubble-asyncapi.yml
- filename: openapi.yaml
  format: yaml
  label: Cilium Operator API
  slug: cilium-operator-api
  spec_type: OpenAPI
  url: https://github.com/cilium/cilium/blob/main/api/v1/operator/openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cilium.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: tetragon.io
  spf: false
hosts:
- cert_expires: Aug 21 19:34:02 2026 GMT
  host: cilium.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 20:32:49 2026 GMT
  host: docs.cilium.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 06:35:25 2026 GMT
  host: tetragon.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cilium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cilium, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cilium
provider_slug: cilium
slug: cilium-domain-security
source_filename: cilium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cilium.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 19:34:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.cilium.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:32:49 2026 GMT\n  hsts: false\n- host: tetragon.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 06:35:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: cilium.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: tetragon.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cilium/refs/heads/main/security/cilium-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Native
- eBPF
- Kubernetes
- Networking
- Security
---
