---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 iodef "mailto:security@eligible.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eligible.com
  spf: true
- caa:
  - 0 iodef "mailto:security@eligible.com"
  - 0 issue "digicert.com"
  - 0 issuewild ";"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eligibleapi.com
  spf: true
hosts:
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: eligible.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 14 23:59:59 2027 GMT
  host: gds.eligibleapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eligible Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eligible, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Eligible
provider_slug: eligible
slug: eligible-domain-security
source_filename: eligible-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eligible.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: null\n- host: gds.eligibleapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: eligible.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:security@eligible.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: eligibleapi.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@eligible.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \";\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eligible/refs/heads/main/security/eligible-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Billing
- Eligibility
- Healthcare
- Insurance
- Claims
---
