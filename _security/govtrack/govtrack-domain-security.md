---
api_specs:
- filename: api
  format: yaml
  label: GovTrack REST API
  slug: govtrack-api
  spec_type: OpenAPI
  url: https://www.govtrack.us/developers/api
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: govtrack.us
  spf: true
hosts:
- cert_expires: Sep 21 12:55:38 2026 GMT
  host: www.govtrack.us
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Govtrack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GovTrack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GovTrack
provider_slug: govtrack
slug: govtrack-domain-security
source_filename: govtrack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.govtrack.us\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 21 12:55:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: govtrack.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/govtrack/refs/heads/main/security/govtrack-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Government
- Legislative
- Congress
- Bills
- Voting Records
- Political Data
- Open Government
- United States
---
