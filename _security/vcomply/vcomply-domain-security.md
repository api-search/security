---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: v-comply.com
  spf: true
hosts:
- cert_expires: Sep 22 03:03:30 2026 GMT
  host: www.v-comply.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vcomply Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VComply, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: VComply
provider_slug: vcomply
slug: vcomply-domain-security
source_filename: vcomply-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.v-comply.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 03:03:30 2026 GMT\n  hsts: false\ndomains:\n- domain: v-comply.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vcomply/refs/heads/main/security/vcomply-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Enterprise
- GRC
- Compliance
- Risk Management
- Policy Management
- Audit
- Incident Management
- SaaS
---
