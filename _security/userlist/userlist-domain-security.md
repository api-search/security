---
api_specs:
- filename: userlist-openapi-generated.yml
  format: yaml
  label: Userlist API
  slug: userlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userlist/openapi/_ae-authored/userlist-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: userlist.com
  spf: true
hosts:
- cert_expires: Dec 27 08:34:04 2026 GMT
  host: userlist.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Userlist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Userlist, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Userlist
provider_slug: userlist
slug: userlist-domain-security
source_filename: userlist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: userlist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 08:34:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: userlist.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/userlist/security/userlist-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Email Marketing
- Software-as-a-Service
- Automation
- Segmentation
- Webhook
- Company
---
