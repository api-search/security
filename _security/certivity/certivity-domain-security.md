---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: certivity.io
  spf: true
hosts:
- cert_expires: Aug 30 04:09:10 2026 GMT
  host: www.certivity.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Certivity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Certivity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Certivity
provider_slug: certivity
slug: certivity-domain-security
source_filename: certivity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.certivity.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 04:09:10 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: certivity.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/certivity/refs/heads/main/security/certivity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Regulatory Technology
- RegTech
- Compliance
- Regulatory Intelligence
- Automotive
- Homologation
- Engineering
- Standards
- Knowledge Graph
- Artificial Intelligence
---
