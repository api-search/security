---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: merlot.org
  spf: true
hosts:
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: merlot.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Merlot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MERLOT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MERLOT
provider_slug: merlot
slug: merlot-domain-security
source_filename: merlot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: merlot.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: merlot.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/merlot/security/merlot-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Education
- Open-Source
- Community
- Learning
---
