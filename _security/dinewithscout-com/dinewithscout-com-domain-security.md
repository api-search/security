---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dinewithscout.com
  spf: true
hosts:
- cert_expires: Dec  8 17:20:10 2026 GMT
  host: dinewithscout.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dinewithscout Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scout, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Scout
provider_slug: dinewithscout-com
slug: dinewithscout-com-domain-security
source_filename: dinewithscout-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dinewithscout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 17:20:10 2026 GMT\n  hsts: false\ndomains:\n- domain: dinewithscout.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dinewithscout-com/security/dinewithscout-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Restaurant
- Reservations
- Automation
- Software-as-a-Service
- Consumer
---
