---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: achurch.ai
  spf: true
hosts:
- cert_expires: Dec 24 18:25:19 2026 GMT
  host: achurch.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Achurch Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for a Church AI + Human, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: a Church AI + Human
provider_slug: achurch-ai
slug: achurch-ai-domain-security
source_filename: achurch-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: achurch.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 18:25:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: achurch.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/achurch-ai/security/achurch-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Spirituality
- Community
- Open Source
- Innovation
---
