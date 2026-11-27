---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: labnotes.org
  spf: true
hosts:
- cert_expires: Dec 29 12:58:30 2026 GMT
  host: labnotes.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Labnotes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Labnotes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Labnotes
provider_slug: labnotes-org
slug: labnotes-org-domain-security
source_filename: labnotes-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: labnotes.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 12:58:30 2026 GMT\n  hsts: false\ndomains:\n- domain: labnotes.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/labnotes-org/security/labnotes-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Newsletters
- Community
- Tech
- Software Design
- Personal Brand
---
