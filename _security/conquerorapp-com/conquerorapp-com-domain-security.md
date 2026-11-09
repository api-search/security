---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: conquerorapp.com
  spf: true
hosts:
- cert_expires: Jan  2 01:05:47 2027 GMT
  host: conquerorapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Conquerorapp Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conqueror, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Conqueror
provider_slug: conquerorapp-com
slug: conquerorapp-com-domain-security
source_filename: conquerorapp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: conquerorapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 01:05:47 2027 GMT\n  hsts: false\ndomains:\n- domain: conquerorapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/conquerorapp-com/security/conquerorapp-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- SEO
- WordPress
- Automation
- AI Agents
---
