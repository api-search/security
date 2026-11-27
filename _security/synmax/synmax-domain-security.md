---
api_specs:
- filename: synmax-openapi-generated.yml
  format: yaml
  label: SynMax (Leviaton) API
  slug: synmax-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synmax/openapi/_ae-authored/synmax-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: synmax.com
  spf: true
hosts:
- cert_expires: Jan  1 03:26:08 2027 GMT
  host: www.synmax.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SynMax (Leviaton) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SynMax (Leviaton), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SynMax (Leviaton)
provider_slug: synmax
slug: synmax-domain-security
source_filename: synmax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.synmax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 03:26:08 2027 GMT\n  hsts: false\ndomains:\n- domain: synmax.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/synmax/security/synmax-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Maritime Intelligence
- Energy Intelligence
- Satellite Data
- AI Analytics
- Vessel Tracking
- Oil & Gas Monitoring
---
