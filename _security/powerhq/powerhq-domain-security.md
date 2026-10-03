---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: powerhq.co
  spf: false
hosts:
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: www.powerhq.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Powerhq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PowerHQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: PowerHQ
provider_slug: powerhq
slug: powerhq-domain-security
source_filename: powerhq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.powerhq.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: powerhq.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/powerhq/refs/heads/main/security/powerhq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy Commerce
- Retail Electricity
- Marketplace
- Energy Providers
- Developers
- Partners
- Brokers
---
