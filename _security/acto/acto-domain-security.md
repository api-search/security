---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: acto.com
  spf: true
hosts:
- cert_expires: Nov 15 07:13:01 2026 GMT
  host: acto.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Acto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ACTO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ACTO
provider_slug: acto
slug: acto-domain-security
source_filename: acto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: acto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 07:13:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: acto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acto/refs/heads/main/security/acto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Life Sciences
- Pharmaceutical
- Sales Enablement
- Learning Management
- Field Force Effectiveness
- Medical Affairs
- Commercial Excellence
- Training and Certification
- Omnichannel Engagement
- Artificial Intelligence
- Medical Devices
- Biotechnology
- Content Management
- Healthcare
---
