---
api_specs:
- filename: patreon-openapi.yml
  format: yaml
  label: Patreon API v2
  slug: patreon-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/patreon/refs/heads/main/openapi/patreon-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: patreon.com
  spf: true
hosts:
- cert_expires: Sep 20 23:28:59 2026 GMT
  host: www.patreon.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 23:28:59 2026 GMT
  host: docs.patreon.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Patreon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Patreon, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Patreon
provider_slug: patreon
slug: patreon-domain-security
source_filename: patreon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.patreon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:28:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.patreon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:28:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: patreon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/patreon/refs/heads/main/security/patreon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Creator Economy
- Membership
- Subscription
- Content
- Community
---
