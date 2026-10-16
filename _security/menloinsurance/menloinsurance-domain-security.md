---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: menloinsurance.com
  spf: true
hosts:
- cert_expires: Dec 29 01:34:50 2026 GMT
  host: www.menloinsurance.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Menloinsurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Menlo Insurance Services, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Menlo Insurance Services
provider_slug: menloinsurance
slug: menloinsurance-domain-security
source_filename: menloinsurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.menloinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 01:34:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: menloinsurance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/menloinsurance/refs/heads/main/security/menloinsurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Brokerage
- Commercial
- Personal
- Quotes
---
