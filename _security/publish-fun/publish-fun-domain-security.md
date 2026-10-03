---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: publish.fun
  spf: true
hosts:
- cert_expires: Dec 26 22:06:11 2026 GMT
  host: publish.fun
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Publish Fun Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Publish.fun, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Publish.fun
provider_slug: publish-fun
slug: publish-fun-domain-security
source_filename: publish-fun-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: publish.fun\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 22:06:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: publish.fun\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/publish-fun/refs/heads/main/security/publish-fun-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Research
- Publishing
- Journals
- Open Science
---
