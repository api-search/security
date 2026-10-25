---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sandfire.com.au
  spf: true
hosts:
- cert_expires: Jan 14 06:28:54 2027 GMT
  host: sandfire.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sandfire Resources Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sandfire Resources, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sandfire Resources
provider_slug: sandfire-resources
slug: sandfire-resources-domain-security
source_filename: sandfire-resources-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sandfire.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 06:28:54 2027 GMT\n  hsts: false\ndomains:\n- domain: sandfire.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sandfire-resources/refs/heads/main/security/sandfire-resources-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Mining
- Copper
- Natural Resources
- Sustainability
- Australia
- ASX Listed
---
