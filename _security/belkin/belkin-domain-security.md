---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issue "starfieldtech.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: belkin.com
  spf: true
hosts:
- cert_expires: Dec 24 09:14:24 2026 GMT
  host: belkin.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Belkin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Belkin WeMo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Belkin WeMo
provider_slug: belkin
slug: belkin-domain-security
source_filename: belkin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: belkin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 09:14:24 2026 GMT\n  hsts: false\ndomains:\n- domain: belkin.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"starfieldtech.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/belkin/security/belkin-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Chargers
- Power Banks
- Phone Cases
- Cables
- Adapters
- Audio
- Screen Protectors
- Surge Protectors
---
