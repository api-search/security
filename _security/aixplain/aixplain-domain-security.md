---
api_specs:
- filename: aixplain-openapi-generated.yml
  format: yaml
  label: aiXplain API
  slug: aixplain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aixplain/refs/heads/main/openapi/_ae-authored/aixplain-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aixplain.com
  spf: true
hosts:
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: www.aixplain.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aixplain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aiXplain, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: aiXplain
provider_slug: aixplain
slug: aixplain-domain-security
source_filename: aixplain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aixplain.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: aixplain.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aixplain/refs/heads/main/security/aixplain-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Artificial Intelligence
- Autonomous-Work
- Enterprise
- Platform
---
