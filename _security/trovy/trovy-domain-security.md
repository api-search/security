---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trovy.com
  spf: true
hosts:
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: trovy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trovy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trovy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Trovy
provider_slug: trovy
slug: trovy-domain-security
source_filename: trovy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trovy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: trovy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trovy/refs/heads/main/security/trovy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- HELOC
- Home Equity
- Credit Cards
- Lending
- Consumer Finance
---
