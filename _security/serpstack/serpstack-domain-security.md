---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: serpstack.com
  spf: true
hosts:
- cert_expires: Oct  6 04:59:30 2026 GMT
  host: serpstack.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Serpstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for serpstack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: serpstack
provider_slug: serpstack
slug: serpstack-domain-security
source_filename: serpstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: serpstack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 04:59:30 2026 GMT\n  hsts: false\ndomains:\n- domain: serpstack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/serpstack/refs/heads/main/security/serpstack-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Development
- Public APIs
---
