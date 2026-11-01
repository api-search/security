---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: comiza.lighting
  spf: true
hosts:
- cert_expires: Dec 13 20:45:30 2026 GMT
  host: comiza.lighting
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Comiza Lighting Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for comiza-lighting, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: comiza-lighting
provider_slug: comiza-lighting
slug: comiza-lighting-domain-security
source_filename: comiza-lighting-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: comiza.lighting\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 20:45:30 2026 GMT\n  hsts: false\ndomains:\n- domain: comiza.lighting\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/comiza-lighting/security/comiza-lighting-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Tools
- Webhooks
- Automation
- Self-hosted
---
