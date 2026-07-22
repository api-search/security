---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: felixpago.com
  spf: true
hosts:
- cert_expires: Sep 22 00:43:05 2026 GMT
  host: www.felixpago.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Felix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Felix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Felix
provider_slug: felix
slug: felix-domain-security
source_filename: felix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.felixpago.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 00:43:05 2026 GMT\n  hsts: false\ndomains:\n- domain: felixpago.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/felix/refs/heads/main/security/felix-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Payments
- Remittances
- Money Transfer
- Latin America
- Financial Services
---
