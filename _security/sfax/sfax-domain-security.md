---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sfax.com
  spf: true
hosts:
- cert_expires: Dec 19 04:12:03 2026 GMT
  host: sfax.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sfax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sfax, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sfax
provider_slug: sfax
slug: sfax-domain-security
source_filename: sfax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sfax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 04:12:03 2026 GMT\n  hsts: null\ndomains:\n- domain: sfax.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/sfax/security/sfax-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
