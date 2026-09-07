---
api_specs:
- filename: zero-networks-platform-openapi.yaml
  format: yaml
  label: Zero Networks Platform API
  slug: zero-networks-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zero-networks/refs/heads/main/openapi/zero-networks-platform-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zeronetworks.com
  spf: true
hosts:
- cert_expires: Oct  3 13:11:46 2026 GMT
  host: zeronetworks.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: portal.zeronetworks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Zero Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zero Networks, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zero Networks
provider_slug: zero-networks
slug: zero-networks-domain-security
source_filename: zero-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zeronetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 13:11:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: portal.zeronetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zeronetworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zero-networks/refs/heads/main/security/zero-networks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- Network Security
- Microsegmentation
- Zero Trust
- Identity
- Multi-Factor Authentication
- Segmentation
- ZTNA
- Kubernetes
- Cybersecurity
---
