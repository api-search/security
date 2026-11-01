---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: outstand.so
  spf: true
hosts:
- cert_expires: Jan 17 16:08:00 2027 GMT
  host: outstand.so
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Outstand So Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for outstand-so, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: outstand-so
provider_slug: outstand-so
slug: outstand-so-domain-security
source_filename: outstand-so-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: outstand.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 16:08:00 2027 GMT\n  hsts: false\ndomains:\n- domain: outstand.so\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/outstand-so/security/outstand-so-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Social Media
- API
- MCP
- SaaS
---
