---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: carpentertechnology.com
  spf: true
hosts:
- cert_expires: Sep 14 20:00:42 2026 GMT
  host: www.carpentertechnology.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carpenter Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carpenter Technology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Carpenter Technology
provider_slug: carpenter-technology
slug: carpenter-technology-domain-security
source_filename: carpenter-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carpentertechnology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 20:00:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: carpentertechnology.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carpenter-technology/refs/heads/main/security/carpenter-technology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Specialty Alloys
- Titanium
- Stainless Steel
- Aerospace
- Defense
- Medical
- Materials Science
- Fortune 1000
---
