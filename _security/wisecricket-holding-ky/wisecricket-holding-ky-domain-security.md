---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wisecricket.ai
  spf: true
hosts:
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: wisecricket.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wisecricket Holding Ky Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WISECRICKET HOLDING KY, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WISECRICKET HOLDING KY
provider_slug: wisecricket-holding-ky
slug: wisecricket-holding-ky-domain-security
source_filename: wisecricket-holding-ky-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wisecricket.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wisecricket.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wisecricket-holding-ky/refs/heads/main/security/wisecricket-holding-ky-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Tax
- Accounting
- Audit
- Artificial Intelligence
- Compliance
- Fintech
---
