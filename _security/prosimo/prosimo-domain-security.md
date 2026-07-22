---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: prosimo.io
  spf: true
hosts:
- cert_expires: Sep  7 08:42:46 2026 GMT
  host: prosimo.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prosimo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prosimo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Prosimo
provider_slug: prosimo
slug: prosimo-domain-security
source_filename: prosimo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prosimo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 08:42:46 2026 GMT\n  hsts: false\ndomains:\n- domain: prosimo.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prosimo/refs/heads/main/security/prosimo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cloud Networking
- Multi-Cloud
- Networking
- Zero Trust
- Security
- Infrastructure as Code
- Terraform
- Cloud Transit
- Observability
---
