---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: anitian.com
  spf: false
hosts:
- cert_expires: Oct 10 21:08:41 2026 GMT
  host: www.anitian.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: securecloud.anitian.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: copilot.anitian.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anitian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anitian, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Anitian
provider_slug: anitian
slug: anitian-domain-security
source_filename: anitian-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anitian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 21:08:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: securecloud.anitian.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: false\n- host: copilot.anitian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: anitian.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anitian/refs/heads/main/security/anitian-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Compliance
- Cloud
- Governance
- FedRAMP
- Government
- Risk
- Audit
- Automation
---
