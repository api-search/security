---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lincolninst.edu
  spf: true
hosts:
- cert_expires: Dec  5 10:15:59 2026 GMT
  host: www.lincolninst.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lincoln Institute Of Land Policy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lincoln Institute of Land Policy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lincoln Institute of Land Policy
provider_slug: lincoln-institute-of-land-policy
slug: lincoln-institute-of-land-policy-domain-security
source_filename: lincoln-institute-of-land-policy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lincolninst.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 10:15:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lincolninst.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lincoln-institute-of-land-policy/security/lincoln-institute-of-land-policy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Research
- LandPolicy
- Nonprofit
- Education
---
