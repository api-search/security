---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: platformable.com
  spf: true
hosts:
- cert_expires: Aug 30 08:02:09 2026 GMT
  host: platformable.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Platformable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Platformable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Platformable
provider_slug: platformable
slug: platformable-domain-security
source_filename: platformable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: platformable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 08:02:09 2026 GMT\n  hsts: false\ndomains:\n- domain: platformable.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/platformable/refs/heads/main/security/platformable-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- API Governance
- Consultancy
- Digital Health
- Ecosystems
- Open Banking
- Open Ecosystems
- Platform
- Traceability
- Training
---
