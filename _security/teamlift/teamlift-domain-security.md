---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: teamlift.co
  spf: true
hosts:
- cert_expires: Dec 22 08:35:00 2026 GMT
  host: www.teamlift.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Teamlift Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TeamLift, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TeamLift
provider_slug: teamlift
slug: teamlift-domain-security
source_filename: teamlift-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.teamlift.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 08:35:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: teamlift.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teamlift/refs/heads/main/security/teamlift-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Training
- Enterprise
- Personalization
- TeamLift
---
