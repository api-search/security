---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: orionlaw.com
  spf: true
hosts:
- cert_expires: Jan 24 19:13:19 2027 GMT
  host: orionlaw.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Orion Law Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orion Law, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Orion Law
provider_slug: orion-law
slug: orion-law-domain-security
source_filename: orion-law-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orionlaw.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 19:13:19 2027 GMT\n  hsts: false\ndomains:\n- domain: orionlaw.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/orion-law/security/orion-law-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Law
- Software
- SaaS
- LegalTech
- Management
---
