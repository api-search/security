---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: kaizan.ai
  spf: true
hosts:
- cert_expires: Jan  3 05:45:37 2027 GMT
  host: kaizan.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kaizan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kaizan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Kaizan
provider_slug: kaizan-ai
slug: kaizan-ai-domain-security
source_filename: kaizan-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kaizan.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 05:45:37 2027 GMT\n  hsts: false\ndomains:\n- domain: kaizan.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/kaizan-ai/security/kaizan-ai-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Client Intelligence
- Customer Success Software
---
