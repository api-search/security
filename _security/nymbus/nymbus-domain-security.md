---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nymbus.com
  spf: true
hosts:
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: nymbus.com
  hsts: true
  hsts_max_age: 525600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nymbus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nymbus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nymbus
provider_slug: nymbus
slug: nymbus-domain-security
source_filename: nymbus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nymbus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 525600\ndomains:\n- domain: nymbus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nymbus/refs/heads/main/security/nymbus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Banking
- Core Banking
- FinTech
- Financial Services
- Banking as a Service
- Digital Banking
- APIs
---
