---
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@heal.com"
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: true
  domain: heal.com
  spf: true
hosts:
- cert_expires: Nov 13 21:29:10 2026 GMT
  host: www.heal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Heal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Heal
provider_slug: heal
slug: heal-domain-security
source_filename: heal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.heal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 21:29:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: heal.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:security@heal.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heal/refs/heads/main/security/heal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Health
- Healthcare
- Telehealth
- Primary Care
- Remote Patient Monitoring
- Medicare
- Home Health
- Acquired
---
