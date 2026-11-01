---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: afroleadership.org
  spf: true
hosts:
- cert_expires: Dec 26 02:40:14 2026 GMT
  host: afroleadership.org
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Afroleadership Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AfroLeadership, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AfroLeadership
provider_slug: afroleadership
slug: afroleadership-domain-security
source_filename: afroleadership-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: afroleadership.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 02:40:14 2026 GMT\n  hsts: null\ndomains:\n- domain: afroleadership.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/afroleadership/security/afroleadership-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- NGO
- Africa
- Transparency
- CivicTech
- DigitalRights
---
