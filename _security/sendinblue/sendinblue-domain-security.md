---
api_specs:
- filename: sendinblue-webhooks-asyncapi.yml
  format: yaml
  label: Sendinblue
  slug: sendinblue
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendinblue/refs/heads/main/asyncapi/sendinblue-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sendinblue.com
  spf: true
hosts:
- cert_expires: Aug 21 22:48:01 2026 GMT
  host: developers.sendinblue.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sendinblue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sendinblue, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Sendinblue
provider_slug: sendinblue
slug: sendinblue-domain-security
source_filename: sendinblue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.sendinblue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 22:48:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sendinblue.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendinblue/refs/heads/main/security/sendinblue-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Email
- Public APIs
---
