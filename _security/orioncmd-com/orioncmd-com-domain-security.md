---
api_specs:
- filename: orioncmd-com-openapi-generated.yml
  format: yaml
  label: OrionCmd API
  slug: orioncmd-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orioncmd-com/openapi/_ae-authored/orioncmd-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: orioncmd.com
  spf: true
hosts:
- cert_expires: Feb 13 07:19:14 2027 GMT
  host: orioncmd.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OrionCmd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OrionCmd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OrionCmd
provider_slug: orioncmd-com
slug: orioncmd-com-domain-security
source_filename: orioncmd-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orioncmd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 07:19:14 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: orioncmd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/orioncmd-com/security/orioncmd-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Monitoring
- Threat Intelligence
- Uptime
- SSL
- DNS
---
