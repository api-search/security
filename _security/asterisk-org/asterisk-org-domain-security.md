---
api_specs:
- filename: asterisk-org-openapi-generated.yml
  format: yaml
  label: Asterisk API
  slug: asterisk-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterisk-org/openapi/_ae-authored/asterisk-org-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: asterisk.org
  spf: true
hosts:
- cert_expires: Dec 31 18:01:44 2026 GMT
  host: asterisk.org
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Asterisk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Asterisk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Asterisk
provider_slug: asterisk-org
slug: asterisk-org-domain-security
source_filename: asterisk-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: asterisk.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 18:01:44 2026 GMT\n  hsts: null\ndomains:\n- domain: asterisk.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/asterisk-org/security/asterisk-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Communications
- Open Source
- Telephony
- VoIP
- Community
---
