---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: grantedhealth.com
  spf: true
hosts:
- cert_expires: Sep 29 21:28:24 2026 GMT
  host: grantedhealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Granted Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Granted, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Granted
provider_slug: granted
slug: granted-domain-security
source_filename: granted-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grantedhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 21:28:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: grantedhealth.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/granted/refs/heads/main/security/granted-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Medical Billing
- Health Insurance
- Consumer
- Artificial Intelligence
---
