---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nibs.org
  spf: true
hosts:
- cert_expires: Dec  9 01:00:08 2026 GMT
  host: www.nibs.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: National Institute Of Building Sciences Nibs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Institute of Building Sciences (NIBS), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: National Institute of Building Sciences (NIBS)
provider_slug: national-institute-of-building-sciences-nibs
slug: national-institute-of-building-sciences-nibs-domain-security
source_filename: national-institute-of-building-sciences-nibs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nibs.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 01:00:08 2026 GMT\n  hsts: false\ndomains:\n- domain: nibs.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/national-institute-of-building-sciences-nibs/security/national-institute-of-building-sciences-nibs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Building Sciences
- Nonprofit
- Research
- Standards
- Education
- Company
---
