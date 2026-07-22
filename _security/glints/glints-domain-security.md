---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: glints.com
  spf: true
hosts:
- cert_expires: Aug 20 00:16:54 2026 GMT
  host: glints.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Glints Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Glints, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Glints
provider_slug: glints
slug: glints-domain-security
source_filename: glints-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: glints.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 00:16:54 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: glints.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glints/refs/heads/main/security/glints-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Enterprise
- Recruitment
- Talent
- Jobs
- Human Resources
- Careers
- Hiring
- Southeast Asia
- Marketplace
---
