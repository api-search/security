---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: simplifeye.co
  spf: true
hosts:
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: www.simplifeye.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simplifeye Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simplifeye, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Simplifeye
provider_slug: simplifeye
slug: simplifeye-domain-security
source_filename: simplifeye-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.simplifeye.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: simplifeye.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simplifeye/refs/heads/main/security/simplifeye-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Dental
- Healthcare
- Payments
- Online Scheduling
- Practice Management
- Patient Engagement
- HIPAA
---
