---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kaimeilabs.dev
  spf: true
hosts:
- cert_expires: Jan 21 14:15:21 2027 GMT
  host: kaimeilabs.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kaimei Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kaimei Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kaimei Labs
provider_slug: kaimeilabs-dev
slug: kaimeilabs-dev-domain-security
source_filename: kaimeilabs-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kaimeilabs.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 14:15:21 2027 GMT\n  hsts: false\ndomains:\n- domain: kaimeilabs.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/kaimeilabs-dev/security/kaimeilabs-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- Verification
- AI Agents
- procedural domain
- Food Tech
- SDK
---
