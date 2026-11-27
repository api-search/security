---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: genppt.com
  spf: true
hosts:
- cert_expires: Jan 31 17:31:02 2027 GMT
  host: genppt.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GenPPT Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GenPPT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GenPPT
provider_slug: genppt
slug: genppt-domain-security
source_filename: genppt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: genppt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 17:31:02 2027 GMT\n  hsts: false\ndomains:\n- domain: genppt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/genppt/security/genppt-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Presentation
- Automation
- Productivity
- Software-as-a-Service
- Company
---
