---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aaisonline.com
  spf: true
hosts:
- cert_expires: Apr  8 23:59:59 2027 GMT
  host: aaisonline.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: American Association of Insurance Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for American Association of Insurance Services, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: American Association of Insurance Services
provider_slug: aais
slug: aais-domain-security
source_filename: aais-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aaisonline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: aaisonline.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/aais/security/aais-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Insurance
- Not-for-profit
- Data Technology
- Advisory Services
- Membership
---
