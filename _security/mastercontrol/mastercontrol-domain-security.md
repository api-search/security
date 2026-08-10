---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mastercontrol.com
  spf: true
hosts:
- cert_expires: Sep  7 01:01:58 2026 GMT
  host: www.mastercontrol.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 22:33:07 2026 GMT
  host: mx.us-west-2.svc.mastercontrol.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mastercontrol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MasterControl, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: MasterControl
provider_slug: mastercontrol
slug: mastercontrol-domain-security
source_filename: mastercontrol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mastercontrol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 01:01:58 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: mx.us-west-2.svc.mastercontrol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 22:33:07 2026 GMT\n  hsts: null\ndomains:\n- domain: mastercontrol.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mastercontrol/refs/heads/main/security/mastercontrol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Quality Management
- Manufacturing
- Life Sciences
- Compliance
- Document Management
- Regulatory
- Enterprise Software
---
