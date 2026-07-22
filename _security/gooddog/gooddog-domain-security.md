---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gooddog.com
  spf: true
hosts:
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: gooddog.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Gooddog Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Good Dog, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Good Dog
provider_slug: gooddog
slug: gooddog-domain-security
source_filename: gooddog-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gooddog.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: gooddog.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gooddog/refs/heads/main/security/gooddog-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Marketplace
- Pets
- Dogs
- Breeders
- Animal Welfare
- Consumer
- Payments
- Pet Insurance
---
