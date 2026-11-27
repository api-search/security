---
description: ''
domains:
- caa:
  - u0awjxny.up.railway.app.
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: outfitmaker.ai
  spf: false
hosts:
- cert_expires: Feb  2 05:29:28 2027 GMT
  host: outfitmaker.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Outfit AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Outfit AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=quarantine).'
provider_name: Outfit AI
provider_slug: outfitmaker-ai
slug: outfitmaker-ai-domain-security
source_filename: outfitmaker-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: outfitmaker.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 05:29:28 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: outfitmaker.ai\n  dnssec: true\n  caa:\n  - u0awjxny.up.railway.app.\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/outfitmaker-ai/security/outfitmaker-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Fashion
- Outfit
- Free
- Web
---
