---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sendjim.com
  spf: true
hosts:
- cert_expires: Dec 29 01:36:13 2026 GMT
  host: sendjim.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sendjim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SendJim, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SendJim
provider_slug: sendjim
slug: sendjim-domain-security
source_filename: sendjim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sendjim.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 01:36:13 2026 GMT\n  hsts: null\ndomains:\n- domain: sendjim.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/sendjim/security/sendjim-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Marketing
- DirectMail
- HomeServices
- Automation
- SaaS
---
