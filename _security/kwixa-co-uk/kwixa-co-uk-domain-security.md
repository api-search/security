---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kwixa.co.uk
  spf: true
hosts:
- cert_expires: Jan 15 20:18:59 2027 GMT
  host: kwixa.co.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kwixa Ltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kwixa Ltd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kwixa Ltd
provider_slug: kwixa-co-uk
slug: kwixa-co-uk-domain-security
source_filename: kwixa-co-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kwixa.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 20:18:59 2027 GMT\n  hsts: false\ndomains:\n- domain: kwixa.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kwixa-co-uk/security/kwixa-co-uk-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Games
- Tools
- United Kingdom
- Free
---
