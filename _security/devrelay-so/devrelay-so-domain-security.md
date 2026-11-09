---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: devrelay.so
  spf: true
hosts:
- cert_expires: Dec 29 09:17:41 2026 GMT
  host: devrelay.so
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Devrelay So Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DevRelay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DevRelay
provider_slug: devrelay-so
slug: devrelay-so-domain-security
source_filename: devrelay-so-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: devrelay.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 09:17:41 2026 GMT\n  hsts: false\ndomains:\n- domain: devrelay.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/devrelay-so/security/devrelay-so-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- DevRel
- Automation
- GitHub
- Content
---
