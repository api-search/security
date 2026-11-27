---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: localimpact.com
  spf: true
hosts:
- cert_expires: Jan 21 05:19:29 2027 GMT
  host: localimpact.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LocalImpact Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LocalImpact, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LocalImpact
provider_slug: localimpact
slug: localimpact-domain-security
source_filename: localimpact-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: localimpact.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 05:19:29 2027 GMT\n  hsts: false\ndomains:\n- domain: localimpact.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/localimpact/security/localimpact-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Review
- Software-as-a-Service
- Local Business
- Reputation
- Software
---
