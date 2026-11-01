---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: iobroker.net
  spf: true
hosts:
- cert_expires: Dec 23 23:06:40 2026 GMT
  host: iobroker.net
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Iobroker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ioBroker (self-hosted), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ioBroker (self-hosted)
provider_slug: iobroker
slug: iobroker-domain-security
source_filename: iobroker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iobroker.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 23 23:06:40 2026 GMT\n  hsts: false\ndomains:\n- domain: iobroker.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/iobroker/security/iobroker-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- IoT
- HomeAutomation
- OpenSource
- IntegrationPlatform
- SelfHosted
---
