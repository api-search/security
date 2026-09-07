---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: xage.com
  spf: true
hosts:
- cert_expires: Nov 24 21:00:29 2026 GMT
  host: xage.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Xage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xage, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Xage
provider_slug: xage
slug: xage-domain-security
source_filename: xage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 21:00:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: xage.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xage/refs/heads/main/security/xage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Cybersecurity
- Zero Trust
- Identity and Access Management
- Privileged Access Management
- Operational Technology
- Critical Infrastructure
- Industrial
- Agent Security
---
