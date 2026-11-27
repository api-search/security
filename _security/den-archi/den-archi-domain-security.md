---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: den.archi
  spf: true
hosts:
- cert_expires: Feb  3 08:08:51 2027 GMT
  host: den.archi
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Den Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Den, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Den
provider_slug: den-archi
slug: den-archi-domain-security
source_filename: den-archi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: den.archi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 08:08:51 2027 GMT\n  hsts: false\ndomains:\n- domain: den.archi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/den-archi/security/den-archi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Architecture
- Construction
- AEC
- Building Codes
- Standards
- Knowledge Base
- MCP
- AI Agents
- South Korea
---
