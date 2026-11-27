---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nyxory.com
  spf: true
hosts:
- cert_expires: Jan 20 19:20:32 2027 GMT
  host: nyxory.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nyxory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nyxory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nyxory
provider_slug: nyxory-com
slug: nyxory-com-domain-security
source_filename: nyxory-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nyxory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 19:20:32 2027 GMT\n  hsts: false\ndomains:\n- domain: nyxory.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nyxory-com/security/nyxory-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Platform
- Agents
- European Infrastructure
- Compliance
---
