---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dns_aid:
    checked: '2026-11-27'
    published: false
  dnssec: false
  domain: tripyana.com
  spf: true
hosts:
- cert_expires: Jan  1 09:00:22 2027 GMT
  host: tripyana.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tripyana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tripyana, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tripyana
provider_slug: tripyana-com
slug: tripyana-com-domain-security
source_filename: tripyana-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tripyana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 09:00:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tripyana.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dns_aid:\n    checked: '2026-11-27'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tripyana-com/security/tripyana-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Chauffeur
- Transportation
- Luxury
- Travel
---
