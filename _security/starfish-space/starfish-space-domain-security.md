---
api_specs:
- filename: starfish-space-wordpress-openapi.yml
  format: yaml
  label: Starfish Space Website Content API
  slug: starfish-space-website-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starfish-space/refs/heads/main/openapi/starfish-space-wordpress-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: starfishspace.com
  spf: true
hosts:
- cert_expires: Sep 27 20:01:16 2026 GMT
  host: www.starfishspace.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Starfish Space Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Starfish Space, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Starfish Space
provider_slug: starfish-space
slug: starfish-space-domain-security
source_filename: starfish-space-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.starfishspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 20:01:16 2026 GMT\n  hsts: false\ndomains:\n- domain: starfishspace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/starfish-space/refs/heads/main/security/starfish-space-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Aerospace
- Space
- Satellites
- Satellite Servicing
- Spacecraft
- Space Robotics
- Defense
- Content Management
- Model Context Protocol
---
