---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: drainprices.co.uk
  spf: true
hosts:
- cert_expires: Jan 10 00:14:49 2027 GMT
  host: drainprices.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Drain Prices Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Drain Prices, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Drain Prices
provider_slug: drainprices-co-uk
slug: drainprices-co-uk-domain-security
source_filename: drainprices-co-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: drainprices.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 00:14:49 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: drainprices.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/drainprices-co-uk/security/drainprices-co-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Plumbing
- Home Services
- United Kingdom
- Pricing
- Drainage
---
