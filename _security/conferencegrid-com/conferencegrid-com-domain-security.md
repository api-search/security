---
description: ''
domains:
- caa:
  - f4fp525m.up.railway.app.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: conferencegrid.com
  spf: true
hosts:
- cert_expires: Jan  2 11:02:41 2027 GMT
  host: conferencegrid.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ConferenceGrid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ConferenceGrid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: ConferenceGrid
provider_slug: conferencegrid-com
slug: conferencegrid-com-domain-security
source_filename: conferencegrid-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: conferencegrid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 11:02:41 2027 GMT\n  hsts: false\ndomains:\n- domain: conferencegrid.com\n  dnssec: true\n  caa:\n  - f4fp525m.up.railway.app.\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/conferencegrid-com/security/conferencegrid-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Conferences
- Event
- Trade Shows
- Sales Intelligence
- B2B
- Sponsorship
- MCP
---
