---
api_specs:
- filename: inamprotocol-org-openapi-generated.yml
  format: yaml
  label: INAM Protocol API
  slug: inamprotocol-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inamprotocol-org/openapi/_ae-authored/inamprotocol-org-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: inamprotocol.org
  spf: true
hosts:
- cert_expires: Jan 21 17:24:11 2027 GMT
  host: inamprotocol.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: INAM Protocol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for INAM Protocol, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: INAM Protocol
provider_slug: inamprotocol-org
slug: inamprotocol-org-domain-security
source_filename: inamprotocol-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inamprotocol.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 17:24:11 2027 GMT\n  hsts: false\ndomains:\n- domain: inamprotocol.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/inamprotocol-org/security/inamprotocol-org-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Security
- Verification
- Open Source
- CLI
---
