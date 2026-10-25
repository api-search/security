---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bellevuegold.com.au
  spf: true
hosts:
- cert_expires: Dec 12 21:20:27 2026 GMT
  host: bellevuegold.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bellevue Gold Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bellevue Gold, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bellevue Gold
provider_slug: bellevue-gold
slug: bellevue-gold-domain-security
source_filename: bellevue-gold-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bellevuegold.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 21:20:27 2026 GMT\n  hsts: false\ndomains:\n- domain: bellevuegold.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bellevue-gold/refs/heads/main/security/bellevue-gold-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Gold Mining
- Mining
- Australia
- ASX Listed
- Western Australia
- Natural Resources
---
