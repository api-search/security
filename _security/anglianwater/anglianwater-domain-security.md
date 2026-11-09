---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: anglianwater.co.uk
  spf: true
hosts:
- cert_expires: Jan 25 13:50:14 2027 GMT
  host: www.anglianwater.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anglianwater Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anglian Water, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Anglian Water
provider_slug: anglianwater
slug: anglianwater-domain-security
source_filename: anglianwater-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anglianwater.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 13:50:14 2027 GMT\n  hsts: null\ndomains:\n- domain: anglianwater.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/anglianwater/security/anglianwater-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Water
- Utilities
- United Kingdom
- Infrastructure
- Public Service
---
