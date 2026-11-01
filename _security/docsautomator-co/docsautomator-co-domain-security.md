---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: docsautomator.co
  spf: true
hosts:
- cert_expires: Dec 19 07:17:21 2026 GMT
  host: docsautomator.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Docsautomator Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for docsautomator-co, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: docsautomator-co
provider_slug: docsautomator-co
slug: docsautomator-co-domain-security
source_filename: docsautomator-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docsautomator.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 07:17:21 2026 GMT\n  hsts: false\ndomains:\n- domain: docsautomator.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/docsautomator-co/security/docsautomator-co-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- DocumentAutomation
- NoCode
- AI
- ESignature
- Integration
---
