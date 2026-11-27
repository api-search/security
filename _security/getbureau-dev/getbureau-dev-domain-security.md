---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getbureau.dev
  spf: true
hosts:
- cert_expires: Dec 30 07:27:41 2026 GMT
  host: getbureau.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bureau Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bureau, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bureau
provider_slug: getbureau-dev
slug: getbureau-dev-domain-security
source_filename: getbureau-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getbureau.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 07:27:41 2026 GMT\n  hsts: false\ndomains:\n- domain: getbureau.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/getbureau-dev/security/getbureau-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Open Source
- Self-Hosted
- Automation
- Agents
---
