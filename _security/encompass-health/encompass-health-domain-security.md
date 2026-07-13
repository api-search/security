---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: encompasshealth.com
  spf: true
hosts:
- cert_expires: Sep 11 11:35:21 2026 GMT
  host: www.encompasshealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: developer.encompasshealth.com
  https: false
- host: api.encompasshealth.com
  https: false
kind: domain-security
layout: security
method: probed
name: Encompass Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Encompass Health, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Encompass Health
provider_slug: encompass-health
slug: encompass-health-domain-security
source_filename: encompass-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.encompasshealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 11:35:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.encompasshealth.com\n  https: false\n- host: api.encompasshealth.com\n  https: false\ndomains:\n- domain: encompasshealth.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/encompass-health/refs/heads/main/security/encompass-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Rehabilitation
---
