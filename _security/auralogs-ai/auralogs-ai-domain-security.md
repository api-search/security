---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: auralogs.ai
  spf: true
hosts:
- cert_expires: Dec  9 17:20:30 2026 GMT
  host: auralogs.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Auralogs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Auralogs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Auralogs
provider_slug: auralogs-ai
slug: auralogs-ai-domain-security
source_filename: auralogs-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: auralogs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 17:20:30 2026 GMT\n  hsts: false\ndomains:\n- domain: auralogs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/auralogs-ai/security/auralogs-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Logging
- Artificial Intelligence
- Monitoring
- SDK
- Production
---
