---
api_specs:
- filename: kerne-fi-openapi-generated.yml
  format: yaml
  label: Kerne API
  slug: kerne-fi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kerne-fi/openapi/_ae-authored/kerne-fi-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kerne.fi
  spf: true
hosts:
- cert_expires: Feb 10 19:36:24 2027 GMT
  host: kerne.fi
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kerne Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kerne, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kerne
provider_slug: kerne-fi
slug: kerne-fi-domain-security
source_filename: kerne-fi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kerne.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 19:36:24 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kerne.fi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kerne-fi/security/kerne-fi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Stablecoins
- Cryptocurrency
- Finance
- Base
- Protocol
---
