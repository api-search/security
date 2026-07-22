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
kind: domain-security
layout: security
method: probed
name: Healthsouth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HealthSouth (Encompass Health), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HealthSouth (Encompass Health)
provider_slug: healthsouth
slug: healthsouth-domain-security
source_filename: healthsouth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.encompasshealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 11:35:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: encompasshealth.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/healthsouth/refs/heads/main/security/healthsouth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Hospitals
- Post-Acute Care
- Rehabilitation
- Fortune 1000
---
