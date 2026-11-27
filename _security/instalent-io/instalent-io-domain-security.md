---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: instalent.io
  spf: true
hosts:
- cert_expires: Dec 29 07:50:13 2026 GMT
  host: instalent.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Instalent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Instalent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Instalent
provider_slug: instalent-io
slug: instalent-io-domain-security
source_filename: instalent-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: instalent.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 07:50:13 2026 GMT\n  hsts: false\ndomains:\n- domain: instalent.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/instalent-io/security/instalent-io-domain-security.yml
summary_line: TLSv1.3
tags:
- Recruiting
- Artificial Intelligence
- Software-as-a-Service
- Candidate Sourcing
- Outreach
---
