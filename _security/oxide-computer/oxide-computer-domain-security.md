---
api_specs:
- filename: oxide-computer-region-api-openapi.json
  format: json
  label: Oxide Region API
  slug: oxide-computer-region-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxide-computer/refs/heads/main/openapi/oxide-computer-region-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oxide.computer
  spf: true
hosts:
- cert_expires: Oct 18 01:56:18 2026 GMT
  host: oxide.computer
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 01:39:57 2026 GMT
  host: docs.oxide.computer
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oxide Computer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oxide, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Oxide
provider_slug: oxide-computer
slug: oxide-computer-domain-security
source_filename: oxide-computer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oxide.computer\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 01:56:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.oxide.computer\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 01:39:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: oxide.computer\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oxide-computer/refs/heads/main/security/oxide-computer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Computing
- Infrastructure
- Compute
- Virtualization
- Networking
- Storage
- Hardware
- On-Premise
- Private Cloud
- Open Source
---
