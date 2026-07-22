---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brimstone.com
  spf: true
hosts:
- cert_expires: Aug 15 00:50:26 2026 GMT
  host: www.brimstone.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brimstone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brimstone, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Brimstone
provider_slug: brimstone
slug: brimstone-domain-security
source_filename: brimstone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brimstone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 00:50:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: brimstone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brimstone/refs/heads/main/security/brimstone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Climate Tech
- Materials
- Cement
- Decarbonization
- Critical Minerals
- Manufacturing
- Heavy Industry
---
