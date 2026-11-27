---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: modkeel.com
  spf: true
hosts:
- cert_expires: Dec 30 01:29:37 2026 GMT
  host: modkeel.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Modkeel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Modkeel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Modkeel
provider_slug: modkeel-com
slug: modkeel-com-domain-security
source_filename: modkeel-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: modkeel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 01:29:37 2026 GMT\n  hsts: false\ndomains:\n- domain: modkeel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/modkeel-com/security/modkeel-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Minecraft
- Modding
- Open Source
- Tooling
- Backup
---
