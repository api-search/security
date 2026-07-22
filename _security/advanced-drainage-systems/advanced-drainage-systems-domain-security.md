---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adspipe.com
  spf: true
hosts:
- cert_expires: Oct 18 01:08:22 2026 GMT
  host: www.adspipe.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Advanced Drainage Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Advanced Drainage Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Advanced Drainage Systems
provider_slug: advanced-drainage-systems
slug: advanced-drainage-systems-domain-security
source_filename: advanced-drainage-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adspipe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 01:08:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: adspipe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advanced-drainage-systems/refs/heads/main/security/advanced-drainage-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Stormwater Management
- Manufacturing
- Water Infrastructure
- Drainage
- Construction
---
