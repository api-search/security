---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: braincube.com
  spf: true
hosts:
- cert_expires: Dec 25 12:54:19 2026 GMT
  host: braincube.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Braincube7F2A Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Braincube7f2a, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Braincube7f2a
provider_slug: braincube7f2a
slug: braincube7f2a-domain-security
source_filename: braincube7f2a-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: braincube.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 12:54:19 2026 GMT\n  hsts: false\ndomains:\n- domain: braincube.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/braincube7f2a/refs/heads/main/security/braincube7f2a-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Industrial AI
- Process Optimization
- Manufacturing
- Real-time Analytics
---
