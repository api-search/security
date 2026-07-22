---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: fortemtech.com
  spf: true
hosts:
- cert_expires: Sep 22 07:49:29 2026 GMT
  host: fortemtech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fortem Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fortem Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Fortem Technologies
provider_slug: fortem-technologies
slug: fortem-technologies-domain-security
source_filename: fortem-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fortemtech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 07:49:29 2026 GMT\n  hsts: false\ndomains:\n- domain: fortemtech.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fortem-technologies/refs/heads/main/security/fortem-technologies-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Counter-Drone
- C-UAS
- Airspace Security
- Defense
- Radar
- Command and Control
- Drone Detection
- Aerospace
---
