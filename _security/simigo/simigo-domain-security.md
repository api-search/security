---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: simigo.ai
  spf: true
hosts:
- cert_expires: Nov 13 16:53:15 2026 GMT
  host: partners.simigo.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Simigo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simigo by Telmobil Inc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Simigo by Telmobil Inc
provider_slug: simigo
slug: simigo-domain-security
source_filename: simigo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: partners.simigo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 16:53:15 2026 GMT\n  hsts: false\ndomains:\n- domain: simigo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simigo/refs/heads/main/security/simigo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Telecommunications
- Platform
- Reseller
- Telmobil
---
