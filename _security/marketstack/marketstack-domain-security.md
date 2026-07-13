---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: marketstack.com
  spf: true
hosts:
- cert_expires: Aug 27 22:59:05 2026 GMT
  host: marketstack.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Marketstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Marketstack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Marketstack
provider_slug: marketstack
slug: marketstack-domain-security
source_filename: marketstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: marketstack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 22:59:05 2026 GMT\n  hsts: false\ndomains:\n- domain: marketstack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/security/marketstack-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Finance
- Public APIs
---
