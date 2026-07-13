---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: railinc.com
  spf: true
hosts:
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: public.railinc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Railinc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Railinc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Railinc
provider_slug: railinc
slug: railinc-domain-security
source_filename: railinc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: public.railinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: railinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/railinc/refs/heads/main/security/railinc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Rail
- Freight
- Logistics
- Transportation
- Supply Chain
---
