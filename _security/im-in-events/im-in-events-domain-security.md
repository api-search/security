---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: im-in.events
  spf: true
hosts:
- cert_expires: Jan 14 01:05:05 2027 GMT
  host: im-in.events
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: I'm In! Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for I''m In!, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: I'm In!
provider_slug: im-in-events
slug: im-in-events-domain-security
source_filename: im-in-events-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: im-in.events\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 01:05:05 2027 GMT\n  hsts: false\ndomains:\n- domain: im-in.events\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/im-in-events/security/im-in-events-domain-security.yml
summary_line: TLSv1.3
tags:
- Event
- Artificial Intelligence
- Sign Up
- Volunteer
- Free
---
