---
api_specs:
- filename: mmwhub-tech-openapi-generated.yml
  format: yaml
  label: MMW API
  slug: mmwhub-tech-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mmwhub-tech/openapi/_ae-authored/mmwhub-tech-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: mmwhub.tech
  spf: true
hosts:
- cert_expires: Dec 22 06:25:46 2026 GMT
  host: mmwhub.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MMW Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MMW, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: MMW
provider_slug: mmwhub-tech
slug: mmwhub-tech-domain-security
source_filename: mmwhub-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mmwhub.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 06:25:46 2026 GMT\n  hsts: false\ndomains:\n- domain: mmwhub.tech\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mmwhub-tech/security/mmwhub-tech-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Memory
- Collaboration
- Software-as-a-Service
---
