---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-27'
    published: false
  dnssec: false
  domain: trustedvillas.co.uk
  spf: true
hosts:
- cert_expires: Feb  8 12:41:29 2027 GMT
  host: trustedvillas.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TrustedVillas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TrustedVillas, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TrustedVillas
provider_slug: trustedvillas-co-uk
slug: trustedvillas-co-uk-domain-security
source_filename: trustedvillas-co-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trustedvillas.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 12:41:29 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trustedvillas.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-27'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/trustedvillas-co-uk/security/trustedvillas-co-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Luxury
- Vacation
- Rentals
- Europe
---
