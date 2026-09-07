---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: securian.com
  spf: true
hosts:
- cert_expires: Nov 23 09:09:28 2026 GMT
  host: www.securian.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Securian Financial Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Securian Financial Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Securian Financial Group
provider_slug: securian-financial-group
slug: securian-financial-group-domain-security
source_filename: securian-financial-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.securian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 09:09:28 2026 GMT\n  hsts: null\ndomains:\n- domain: securian.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/securian-financial-group/refs/heads/main/security/securian-financial-group-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fortune 1000
- Financial Services
- Insurance
- Life Insurance
- Annuities
- Retirement
- Group Benefits
- Employee Benefits
---
