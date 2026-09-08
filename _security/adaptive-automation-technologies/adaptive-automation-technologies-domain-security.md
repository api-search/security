---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adaptive.live
  spf: true
hosts:
- cert_expires: Nov 27 09:07:35 2026 GMT
  host: adaptive.live
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 18:07:50 2026 GMT
  host: documentation.adaptive.live
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: app.adaptive.live
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Adaptive Automation Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adaptive Automation Technologies, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Adaptive Automation Technologies
provider_slug: adaptive-automation-technologies
slug: adaptive-automation-technologies-domain-security
source_filename: adaptive-automation-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adaptive.live\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 09:07:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: documentation.adaptive.live\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 18:07:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.adaptive.live\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: adaptive.live\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adaptive-automation-technologies/refs/heads/main/security/adaptive-automation-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Privileged Access Management
- Identity and Access Management
- Data Security
- Agents
- Model Context Protocol
- Infrastructure
- Databases
- Kubernetes
- Compliance
- Audit
---
