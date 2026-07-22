---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: turbine.ai
  spf: true
hosts:
- cert_expires: Sep 28 18:11:52 2026 GMT
  host: turbine.ai
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Turbine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Turbine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Turbine
provider_slug: turbine
slug: turbine-domain-security
source_filename: turbine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: turbine.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 28 18:11:52 2026 GMT\n  hsts: false\ndomains:\n- domain: turbine.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turbine/refs/heads/main/security/turbine-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Biotechnology
- Drug Discovery
- Artificial Intelligence
- Life Sciences
- Simulation
---
