---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: deckspace.org
  spf: true
hosts:
- cert_expires: Jan 15 11:49:25 2027 GMT
  host: deckspace.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Deckspace Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DeckSpace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: DeckSpace
provider_slug: deckspace-org
slug: deckspace-org-domain-security
source_filename: deckspace-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deckspace.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 11:49:25 2027 GMT\n  hsts: false\ndomains:\n- domain: deckspace.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/deckspace-org/security/deckspace-org-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- Presentations
- Diagramming
- Dashboards
- Collaboration
---
