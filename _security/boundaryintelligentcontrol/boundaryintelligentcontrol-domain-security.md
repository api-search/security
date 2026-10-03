---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: boundarycontrol.com
  spf: true
hosts:
- cert_expires: Dec  7 15:11:57 2026 GMT
  host: www.boundarycontrol.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Boundaryintelligentcontrol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boundaryintelligentcontrol, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Boundaryintelligentcontrol
provider_slug: boundaryintelligentcontrol
slug: boundaryintelligentcontrol-domain-security
source_filename: boundaryintelligentcontrol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.boundarycontrol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 15:11:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: boundarycontrol.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boundaryintelligentcontrol/refs/heads/main/security/boundaryintelligentcontrol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Governance
- DataPrivacy
- Enterprise
- Platform
---
