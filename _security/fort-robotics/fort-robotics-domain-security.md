---
api_specs:
- filename: fort-robotics-openapi-generated.yml
  format: yaml
  label: Fort Robotics API
  slug: fort-robotics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fort-robotics/refs/heads/main/openapi/_ae-authored/fort-robotics-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fortrobotics.com
  spf: true
hosts:
- cert_expires: Nov 17 23:29:44 2026 GMT
  host: www.fortrobotics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fort Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fort Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fort Robotics
provider_slug: fort-robotics
slug: fort-robotics-domain-security
source_filename: fort-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fortrobotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:29:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fortrobotics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fort-robotics/refs/heads/main/security/fort-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Robotics
- Artificial Intelligence
- Safety
- Platform
---
