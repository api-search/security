---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: velocity.tech
  spf: true
hosts:
- cert_expires: Sep 13 00:30:27 2026 GMT
  host: velocity.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Velocity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Velocity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Velocity
provider_slug: velocity
slug: velocity-domain-security
source_filename: velocity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: velocity.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 00:30:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: velocity.tech\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/velocity/refs/heads/main/security/velocity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Devops
- SRE
- Incident Management
- Developer Environments
- AIOps
- Acquired
- Israel
---
