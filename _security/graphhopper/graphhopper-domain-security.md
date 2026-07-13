---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: graphhopper.com
  spf: true
hosts:
- cert_expires: Sep 26 22:25:28 2026 GMT
  host: docs.graphhopper.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Graphhopper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GraphHopper, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GraphHopper
provider_slug: graphhopper
slug: graphhopper-domain-security
source_filename: graphhopper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.graphhopper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 22:25:28 2026 GMT\n  hsts: false\ndomains:\n- domain: graphhopper.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graphhopper/refs/heads/main/security/graphhopper-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Transportation
- Public APIs
---
