---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: excaliclaw.com
  spf: true
hosts:
- cert_expires: Dec 28 19:43:32 2026 GMT
  host: excaliclaw.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ExcaliClaw Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ExcaliClaw, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ExcaliClaw
provider_slug: excaliclaw-com
slug: excaliclaw-com-domain-security
source_filename: excaliclaw-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: excaliclaw.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 19:43:32 2026 GMT\n  hsts: false\ndomains:\n- domain: excaliclaw.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/excaliclaw-com/security/excaliclaw-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Collaboration
- Diagram
- Artificial Intelligence
- Workspace
- Real-Time
---
