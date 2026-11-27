---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: justpublish.ai
  spf: false
hosts:
- cert_expires: Jan 30 13:32:34 2027 GMT
  host: justpublish.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Just Publish Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Just Publish, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Just Publish
provider_slug: justpublish-ai
slug: justpublish-ai-domain-security
source_filename: justpublish-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: justpublish.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 13:32:34 2027 GMT\n  hsts: false\ndomains:\n- domain: justpublish.ai\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/justpublish-ai/security/justpublish-ai-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Artificial Intelligence
- Websites
- Hosting
- Software-as-a-Service
- Publishing
---
