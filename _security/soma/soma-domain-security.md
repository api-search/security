---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: somainsure.com
  spf: true
hosts:
- cert_expires: Oct 17 14:31:02 2026 GMT
  host: www.somainsure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Soma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Soma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Soma
provider_slug: soma
slug: soma-domain-security
source_filename: soma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.somainsure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 14:31:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: somainsure.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soma/refs/heads/main/security/soma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Insurance Tech
- Insurance
- Commercial Insurance
- Insurance Brokerage
- Cyber Liability
- Fintech
---
