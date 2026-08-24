---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jettiresources.com
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: www.jettiresources.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jetti Resources Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jetti Resources, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Jetti Resources
provider_slug: jetti-resources
slug: jetti-resources-domain-security
source_filename: jetti-resources-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jettiresources.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: jettiresources.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jetti-resources/refs/heads/main/security/jetti-resources-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Mining
- Copper
- Critical Minerals
- Metals
- Hydrometallurgy
- Cleantech
- Energy Transition
- Sustainability
- Industrial Technology
---
