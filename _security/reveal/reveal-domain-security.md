---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: reveal.co
  spf: true
hosts:
- cert_expires: Oct 11 21:30:52 2026 GMT
  host: www.reveal.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reveal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reveal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Reveal
provider_slug: reveal
slug: reveal-domain-security
source_filename: reveal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reveal.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 21:30:52 2026 GMT\n  hsts: null\ndomains:\n- domain: reveal.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reveal/refs/heads/main/security/reveal-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---
