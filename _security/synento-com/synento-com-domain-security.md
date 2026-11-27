---
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@synento.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: synento.com
  spf: true
hosts:
- cert_expires: Jan  1 04:46:35 2027 GMT
  host: synento.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Synento Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synento, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Synento
provider_slug: synento-com
slug: synento-com-domain-security
source_filename: synento-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: synento.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 04:46:35 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: synento.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:security@synento.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/synento-com/security/synento-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Video
- WebRTC
- WebCodecs
- WebSocket
- Streaming
---
