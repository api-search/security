---
description: ''
domains:
- caa:
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "pki.goog"
  - 0 issue "digicert.com"
  dmarc: false
  dnssec: false
  domain: filmtrack.com
  spf: true
hosts:
- host: filmtrack.com
  https: false
kind: domain-security
layout: security
method: probed
name: Filmtrack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FilmTrack, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: FilmTrack
provider_slug: filmtrack
slug: filmtrack-domain-security
source_filename: filmtrack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: filmtrack.com\n  https: false\ndomains:\n- domain: filmtrack.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/filmtrack/refs/heads/main/security/filmtrack-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Entertainment
- Media and Entertainment
- Rights Management
- Royalties
- Licensing
- Content Management
- Intellectual Property
- Contracts
- Revenue Recognition
---
