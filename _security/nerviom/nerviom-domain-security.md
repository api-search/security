---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nerviom.com
  spf: true
hosts:
- cert_expires: Sep 22 05:37:05 2026 GMT
  host: www.nerviom.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nerviom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nerviom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nerviom
provider_slug: nerviom
slug: nerviom-domain-security
source_filename: nerviom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nerviom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 05:37:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nerviom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nerviom/refs/heads/main/security/nerviom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Infrastructure
- Data Centers
- Energy
- Predevelopment
- Workflow Automation
- Site Selection
---
