---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: minairal.com
  spf: true
hosts:
- cert_expires: Dec 31 02:25:01 2026 GMT
  host: minairal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Minairal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Minairal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Minairal
provider_slug: minairal-com
slug: minairal-com-domain-security
source_filename: minairal-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: minairal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 02:25:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: minairal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/minairal-com/security/minairal-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Water dispensers
- Atmospheric water generators
- Reverse Osmosis
- Hotel water systems
- Office water systems
- Villa water systems
- Thailand
---
