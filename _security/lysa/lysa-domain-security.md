---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lysa.se
  spf: true
hosts:
- cert_expires: Nov 29 14:32:50 2026 GMT
  host: lysa.se
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lysa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lysa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lysa
provider_slug: lysa
slug: lysa-domain-security
source_filename: lysa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lysa.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 14:32:50 2026 GMT\n  hsts: false\ndomains:\n- domain: lysa.se\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lysa/refs/heads/main/security/lysa-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fintech
- Investment
- savings
- Automation
- Sweden
- Company
---
