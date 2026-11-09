---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: calvix.io
  spf: true
hosts:
- cert_expires: Jan  9 01:49:28 2027 GMT
  host: calvix.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Calvix Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Calvix Technology Solutions LLC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Calvix Technology Solutions LLC
provider_slug: calvix-io
slug: calvix-io-domain-security
source_filename: calvix-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: calvix.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 01:49:28 2027 GMT\n  hsts: false\ndomains:\n- domain: calvix.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/calvix-io/security/calvix-io-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Managed IT
- Cybersecurity
- Networking
- Automation
- Web Development
---
