---
api_specs:
- filename: simplemdm-openapi-generated.yml
  format: yaml
  label: SimpleMDM API
  slug: simplemdm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simplemdm/openapi/_ae-authored/simplemdm-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: simplemdm.com
  spf: true
hosts:
- cert_expires: Jan 14 18:55:25 2027 GMT
  host: simplemdm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Simplemdm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SimpleMDM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: SimpleMDM
provider_slug: simplemdm
slug: simplemdm-domain-security
source_filename: simplemdm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: simplemdm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 18:55:25 2027 GMT\n  hsts: false\ndomains:\n- domain: simplemdm.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/simplemdm/security/simplemdm-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Mobile Device Management
- Apple
- MDM
- Enterprise
- SaaS
- Company
---
