---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: slurpit.io
  spf: true
hosts:
- cert_expires: Nov 24 13:11:35 2026 GMT
  host: slurpit.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Slurpit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Slurp''it, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Slurp'it
provider_slug: slurpit
slug: slurpit-domain-security
source_filename: slurpit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: slurpit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 13:11:35 2026 GMT\n  hsts: false\ndomains:\n- domain: slurpit.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/slurpit/security/slurpit-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Networks
- Automation
- Open Source
- Documentation
---
