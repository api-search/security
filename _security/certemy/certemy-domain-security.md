---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: certemy.com
  spf: true
hosts:
- cert_expires: Nov 13 23:36:45 2026 GMT
  host: certemy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Certemy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Certemy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Certemy
provider_slug: certemy
slug: certemy-domain-security
source_filename: certemy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: certemy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:36:45 2026 GMT\n  hsts: false\ndomains:\n- domain: certemy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/certemy/refs/heads/main/security/certemy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Workforce Compliance
- License Management
- Credential Verification
- Employee Onboarding
- HRIS Integration
- Enterprise Software
---
