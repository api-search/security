---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cardconnect.com
  spf: true
hosts:
- cert_expires: Apr 22 23:59:59 2027 GMT
  host: cardconnect.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cardconnect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CardConnect (Fiserv), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CardConnect (Fiserv)
provider_slug: cardconnect
slug: cardconnect-domain-security
source_filename: cardconnect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cardconnect.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr 22 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: cardconnect.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/cardconnect/security/cardconnect-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
---
