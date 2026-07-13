---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jobvite.com
  spf: true
hosts:
- cert_expires: Sep 25 06:19:11 2026 GMT
  host: www.jobvite.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 04:48:37 2026 GMT
  host: help.jobvite.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 30 23:59:59 2026 GMT
  host: api.jobvite.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Jobvite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jobvite, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Jobvite
provider_slug: jobvite
slug: jobvite-domain-security
source_filename: jobvite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jobvite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 06:19:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: help.jobvite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 04:48:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.jobvite.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: jobvite.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jobvite/refs/heads/main/security/jobvite-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Applicant Tracking
- ATS
- Recruiting
- Human Resources
- Talent Acquisition
- Onboarding
---
