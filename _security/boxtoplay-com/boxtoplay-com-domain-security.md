---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: boxtoplay.com
  spf: true
hosts:
- cert_expires: Jan 27 17:27:45 2027 GMT
  host: boxtoplay.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BoxToPlay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BoxToPlay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: BoxToPlay
provider_slug: boxtoplay-com
slug: boxtoplay-com-domain-security
source_filename: boxtoplay-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boxtoplay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 17:27:45 2027 GMT\n  hsts: false\ndomains:\n- domain: boxtoplay.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/boxtoplay-com/security/boxtoplay-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Hosting
- Gaming
- Minecraft
- VPS
- TeamSpeak
---
