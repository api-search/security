---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: genstaq.ai
  spf: true
hosts:
- cert_expires: Dec 23 18:50:27 2026 GMT
  host: genstaq.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Genstaq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GenStaq.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GenStaq.ai
provider_slug: genstaq
slug: genstaq-domain-security
source_filename: genstaq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: genstaq.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 18:50:27 2026 GMT\n  hsts: false\ndomains:\n- domain: genstaq.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genstaq/refs/heads/main/security/genstaq-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Infrastructure
- Enterprise
- GenAI
---
