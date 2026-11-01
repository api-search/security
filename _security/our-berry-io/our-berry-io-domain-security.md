---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: our-berry.io
  spf: false
hosts:
- cert_expires: Jan 15 09:37:09 2027 GMT
  host: our-berry.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Our Berry Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Berry Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Berry Health
provider_slug: our-berry-io
slug: our-berry-io-domain-security
source_filename: our-berry-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: our-berry.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 09:37:09 2027 GMT\n  hsts: false\ndomains:\n- domain: our-berry.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/our-berry-io/security/our-berry-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health
- API
- Platform
- Data
---
