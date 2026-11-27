---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oeradio.at
  spf: true
hosts:
- cert_expires: Dec 28 02:55:16 2026 GMT
  host: oeradio.at
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OERadio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OERadio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OERadio
provider_slug: oeradio-at
slug: oeradio-at-domain-security
source_filename: oeradio-at-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oeradio.at\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 02:55:16 2026 GMT\n  hsts: false\ndomains:\n- domain: oeradio.at\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/oeradio-at/security/oeradio-at-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Amateur Radio
- Community
- Tutorials
- Open Source
- Education
---
