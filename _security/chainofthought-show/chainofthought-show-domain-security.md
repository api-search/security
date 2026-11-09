---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chainofthought.show
  spf: false
hosts:
- cert_expires: Jan  6 05:26:38 2027 GMT
  host: chainofthought.show
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chainofthought Show Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chain of Thought, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Chain of Thought
provider_slug: chainofthought-show
slug: chainofthought-show-domain-security
source_filename: chainofthought-show-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chainofthought.show\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 05:26:38 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: chainofthought.show\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/chainofthought-show/security/chainofthought-show-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Podcasts
- Artificial Intelligence
- Infrastructure
- Technology
- Community
---
