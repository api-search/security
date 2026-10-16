---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: filehub.one
  spf: true
hosts:
- cert_expires: Dec  2 01:07:59 2026 GMT
  host: filehub.one
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Filehub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for filehub GmbH, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: filehub GmbH
provider_slug: filehub
slug: filehub-domain-security
source_filename: filehub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: filehub.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 01:07:59 2026 GMT\n  hsts: false\ndomains:\n- domain: filehub.one\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/filehub/refs/heads/main/security/filehub-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Automation
- Document Management
- Finance
- Procurement
- SaaS
---
