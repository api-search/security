---
api_specs:
- filename: passbolt-openapi.yaml
  format: yaml
  label: Passbolt API
  slug: passbolt
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passbolt/refs/heads/main/openapi/passbolt-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: passbolt.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: passbolt.local
  spf: false
hosts:
- cert_expires: Aug 13 01:31:29 2026 GMT
  host: www.passbolt.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: passbolt.local
  https: false
kind: domain-security
layout: security
method: probed
name: Passbolt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Passbolt, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Passbolt
provider_slug: passbolt
slug: passbolt-domain-security
source_filename: passbolt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.passbolt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 01:31:29 2026 GMT\n  hsts: null\n- host: passbolt.local\n  https: false\ndomains:\n- domain: passbolt.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: passbolt.local\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/passbolt/refs/heads/main/security/passbolt-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Password Manager
- Security
- Secrets
- Identity
---
