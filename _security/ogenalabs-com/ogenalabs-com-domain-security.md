---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ogenalabs.com
  spf: true
hosts:
- cert_expires: Dec  7 09:43:52 2026 GMT
  host: ogenalabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ogenalabs Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ogenalabs-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ogenalabs-com
provider_slug: ogenalabs-com
slug: ogenalabs-com-domain-security
source_filename: ogenalabs-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ogenalabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 09:43:52 2026 GMT\n  hsts: false\ndomains:\n- domain: ogenalabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ogenalabs-com/security/ogenalabs-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Automation
- Blockchain
- Security
- Platform
---
