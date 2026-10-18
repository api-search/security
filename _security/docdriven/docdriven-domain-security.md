---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: docdriven.com
  spf: true
hosts:
- cert_expires: Dec 15 18:26:21 2026 GMT
  host: docdriven.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Docdriven Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DocDriven, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DocDriven
provider_slug: docdriven
slug: docdriven-domain-security
source_filename: docdriven-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docdriven.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 18:26:21 2026 GMT\n  hsts: false\ndomains:\n- domain: docdriven.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docdriven/refs/heads/main/security/docdriven-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- API Design
- Artificial Intelligence
- Collaboration
- Documentation
- Platform
---
