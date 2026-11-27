---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: orgsdk.ai
  spf: false
hosts:
- cert_expires: Jan  2 05:04:05 2027 GMT
  host: orgsdk.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OrgSDK Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OrgSDK, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: OrgSDK
provider_slug: orgsdk-ai
slug: orgsdk-ai-domain-security
source_filename: orgsdk-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orgsdk.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 05:04:05 2027 GMT\n  hsts: false\ndomains:\n- domain: orgsdk.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/orgsdk-ai/security/orgsdk-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Platform
- Local
- Open Source
- Automation
---
