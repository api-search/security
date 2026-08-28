---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: regentcraft.com
  spf: true
hosts:
- cert_expires: Sep 30 17:45:55 2026 GMT
  host: www.regentcraft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Regent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for REGENT Craft, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: REGENT Craft
provider_slug: regent
slug: regent-domain-security
source_filename: regent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.regentcraft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 17:45:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: regentcraft.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regent/refs/heads/main/security/regent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Transportation
- Maritime
- Aviation
- Electric Vehicles
- Defense
- Manufacturing
- Mobility
---
