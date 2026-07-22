---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: coso.org
  spf: false
hosts:
- cert_expires: Sep 14 00:40:36 2026 GMT
  host: www.coso.org
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Internal Control Standards Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Internal Control Standards, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Internal Control Standards
provider_slug: internal-control-standards
slug: internal-control-standards-domain-security
source_filename: internal-control-standards-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coso.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 00:40:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: coso.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/internal-control-standards/refs/heads/main/security/internal-control-standards-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Auditing
- Compliance
- COSO
- Governance
- Internal Controls
- Risk Management
- SOX
---
