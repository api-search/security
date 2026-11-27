---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: netfiscus.com
  spf: true
hosts:
- cert_expires: Feb  6 13:48:33 2027 GMT
  host: netfiscus.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NetFiscus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NetFiscus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NetFiscus
provider_slug: netfiscus-com
slug: netfiscus-com-domain-security
source_filename: netfiscus-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: netfiscus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 13:48:33 2027 GMT\n  hsts: false\ndomains:\n- domain: netfiscus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/netfiscus-com/security/netfiscus-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Personal Finance
- Wealth tracking
- AI Assistant
- Multi-Currency
---
