---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openrouteservice.org
  spf: false
hosts:
- cert_expires: Sep 29 19:46:29 2026 GMT
  host: openrouteservice.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openrouteservice Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for openrouteservice.org, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: openrouteservice.org
provider_slug: openrouteservice-org
slug: openrouteservice-org-domain-security
source_filename: openrouteservice-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openrouteservice.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 19:46:29 2026 GMT\n  hsts: false\ndomains:\n- domain: openrouteservice.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openrouteservice-org/refs/heads/main/security/openrouteservice-org-domain-security.yml
summary_line: TLSv1.3
tags:
- Geocoding
- Public APIs
---
