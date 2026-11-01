---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: connectedpaths.com
  spf: true
hosts:
- cert_expires: Jan 23 05:53:58 2027 GMT
  host: connectedpaths.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Connectedpaths Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for connectedpaths-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: connectedpaths-com
provider_slug: connectedpaths-com
slug: connectedpaths-com-domain-security
source_filename: connectedpaths-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: connectedpaths.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 05:53:58 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: connectedpaths.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/connectedpaths-com/security/connectedpaths-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Consultancy
- Strategy
- Implementation
- CEO
- London
---
