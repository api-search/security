---
api_specs:
- filename: netwrix-openapi-generated.yml
  format: yaml
  label: Netwrix API
  slug: netwrix-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netwrix/refs/heads/main/openapi/_ae-authored/netwrix-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: netwrix.com
  spf: true
hosts:
- cert_expires: Nov  9 04:23:49 2026 GMT
  host: www.netwrix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Netwrix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Netwrix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Netwrix
provider_slug: netwrix
slug: netwrix-domain-security
source_filename: netwrix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.netwrix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 04:23:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: netwrix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netwrix/refs/heads/main/security/netwrix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- DataSecurity
- Governance
- Compliance
- PrivilegedAccess
---
