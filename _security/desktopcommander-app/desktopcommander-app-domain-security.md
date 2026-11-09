---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: desktopcommander.app
  spf: true
hosts:
- cert_expires: Jan  1 12:52:09 2027 GMT
  host: desktopcommander.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Desktopcommander App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Desktop Commander, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Desktop Commander
provider_slug: desktopcommander-app
slug: desktopcommander-app-domain-security
source_filename: desktopcommander-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: desktopcommander.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 12:52:09 2027 GMT\n  hsts: false\ndomains:\n- domain: desktopcommander.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/desktopcommander-app/security/desktopcommander-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Automation
- Desktop
- Productivity
- ChatGPT
- Company
---
