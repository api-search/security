---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: compliancequest.com
  spf: true
hosts:
- cert_expires: Jan  3 12:52:20 2027 GMT
  host: www.compliancequest.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Compliancequest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ComplianceQuest, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ComplianceQuest
provider_slug: compliancequest
slug: compliancequest-domain-security
source_filename: compliancequest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.compliancequest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 12:52:20 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: compliancequest.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/compliancequest/refs/heads/main/security/compliancequest-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- PLM
- Quality Management
- EHS
- Supplier Risk
---
