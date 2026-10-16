---
api_specs:
- filename: kontainer-openapi-generated.yml
  format: yaml
  label: Kontainer DAM & PIM API
  slug: kontainer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontainer/refs/heads/main/openapi/_ae-authored/kontainer-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: kontainer.com
  spf: true
hosts:
- cert_expires: Jan  1 02:20:17 2027 GMT
  host: kontainer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kontainer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kontainer DAM & PIM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Kontainer DAM & PIM
provider_slug: kontainer
slug: kontainer-domain-security
source_filename: kontainer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kontainer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 02:20:17 2027 GMT\n  hsts: false\ndomains:\n- domain: kontainer.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kontainer/refs/heads/main/security/kontainer-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- DAM
- PIM
- Digital Asset Management
- Product Information Management
- Asset Management
---
