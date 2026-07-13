---
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@eligible.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eligible.com
  spf: true
hosts:
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: eligible.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eligible Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eligible, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Eligible
provider_slug: eligible
slug: eligible-domain-security
source_filename: eligible-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eligible.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: eligible.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@eligible.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eligible/refs/heads/main/security/eligible-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Billing
- Eligibility
- Healthcare
- Insurance
- Claims
---
