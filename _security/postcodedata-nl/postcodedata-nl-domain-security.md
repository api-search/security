---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: postcodedata.nl
  spf: false
hosts:
- host: api.postcodedata.nl
  https: false
kind: domain-security
layout: security
method: probed
name: Postcodedata Nl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PostcodeData.nl, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: PostcodeData.nl
provider_slug: postcodedata-nl
slug: postcodedata-nl-domain-security
source_filename: postcodedata-nl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.postcodedata.nl\n  https: false\ndomains:\n- domain: postcodedata.nl\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postcodedata-nl/refs/heads/main/security/postcodedata-nl-domain-security.yml
summary_line: DNSSEC
tags:
- Geocoding
- Public APIs
---
