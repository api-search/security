---
api_specs:
- filename: crispy-sh-openapi-generated.yml
  format: yaml
  label: crispy-sh API
  slug: crispy-sh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crispy-sh/openapi/_ae-authored/crispy-sh-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: crispy.sh
  spf: true
hosts:
- cert_expires: Jan 19 20:33:09 2027 GMT
  host: crispy.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crispy Sh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for crispy-sh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: crispy-sh
provider_slug: crispy-sh
slug: crispy-sh-domain-security
source_filename: crispy-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crispy.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 20:33:09 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: crispy.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/crispy-sh/security/crispy-sh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- LinkedIn
- Founders
- Outreach
- Automation
- SaaS
---
