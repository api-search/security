---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ducks.org
  spf: true
hosts:
- cert_expires: Sep 21 11:26:28 2026 GMT
  host: gis.ducks.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ducks Unlimited Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ducks Unlimited, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ducks Unlimited
provider_slug: ducks-unlimited
slug: ducks-unlimited-domain-security
source_filename: ducks-unlimited-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gis.ducks.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 11:26:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ducks.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ducks-unlimited/refs/heads/main/security/ducks-unlimited-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Geocoding
- Public APIs
---
