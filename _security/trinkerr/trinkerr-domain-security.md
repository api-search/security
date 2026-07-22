---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: trinkerr.com
  spf: true
hosts:
- cert_expires: Oct  1 05:31:31 2026 GMT
  host: www.trinkerr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trinkerr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trinkerr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Trinkerr
provider_slug: trinkerr
slug: trinkerr-domain-security
source_filename: trinkerr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trinkerr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 05:31:31 2026 GMT\n  hsts: false\ndomains:\n- domain: trinkerr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trinkerr/refs/heads/main/security/trinkerr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cloud Saas
- Trading
- Algorithmic Trading
- Fintech
- India
- Stock Market
---
