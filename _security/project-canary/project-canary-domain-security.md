---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: projectcanary.com
  spf: true
hosts:
- cert_expires: Sep 16 09:37:41 2026 GMT
  host: www.projectcanary.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Project Canary Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Project Canary, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Project Canary
provider_slug: project-canary
slug: project-canary-domain-security
source_filename: project-canary-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.projectcanary.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 09:37:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: projectcanary.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/project-canary/refs/heads/main/security/project-canary-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Climate Technology
- Emissions
- Methane
- Energy
- Oil and Gas
- Utilities
- Environmental Data
- Sustainability
---
