---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "globalsign.com"
  - 0 issue "globalsign.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: arm.com
  spf: true
hosts:
- cert_expires: Oct 28 10:21:06 2026 GMT
  host: www.arm.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Arm
provider_slug: arm
slug: arm-domain-security
source_filename: arm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 10:21:06 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: arm.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arm/refs/heads/main/security/arm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Semiconductors
- Chip Design
- Processor IP
- Arm Architecture
- Embedded
- Edge AI
- Frontier Tech
---
