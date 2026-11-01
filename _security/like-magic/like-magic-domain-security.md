---
api_specs:
- filename: like-magic-openapi-generated.yml
  format: yaml
  label: LIKE MAGIC API
  slug: like-magic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/like-magic/openapi/_ae-authored/like-magic-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: likemagic.tech
  spf: true
hosts:
- cert_expires: Dec  1 12:19:46 2026 GMT
  host: likemagic.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Like Magic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LIKE MAGIC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LIKE MAGIC
provider_slug: like-magic
slug: like-magic-domain-security
source_filename: like-magic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: likemagic.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 12:19:46 2026 GMT\n  hsts: false\ndomains:\n- domain: likemagic.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/like-magic/security/like-magic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Hospitality
- Technology
- Guest Experience
- Hotel Operations
---
