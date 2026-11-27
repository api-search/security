---
api_specs:
- filename: 3dtexel-com-openapi-generated.yml
  format: yaml
  label: 3DTexel API
  slug: 3dtexel-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3dtexel-com/openapi/_ae-authored/3dtexel-com-openapi-generated.yml
- filename: 3dtexel-com-public-openapi.json
  format: json
  label: 3DTexel public API API
  slug: 3dtexel-public-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3dtexel-com/openapi/_original/3dtexel-com-public-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 3dtexel.com
  spf: true
hosts:
- cert_expires: Dec 17 19:17:00 2026 GMT
  host: 3dtexel.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 3DTexel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 3DTexel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 3DTexel
provider_slug: 3dtexel-com
slug: 3dtexel-com-domain-security
source_filename: 3dtexel-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 3dtexel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 19:17:00 2026 GMT\n  hsts: false\ndomains:\n- domain: 3dtexel.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/3dtexel-com/security/3dtexel-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- 3D Assets
- Textures
- Game Development
---
