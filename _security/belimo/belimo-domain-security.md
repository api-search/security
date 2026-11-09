---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: belimo.com
  spf: true
hosts:
- cert_expires: Dec  7 09:03:39 2026 GMT
  host: www.belimo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Belimo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Belimo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Belimo
provider_slug: belimo
slug: belimo-domain-security
source_filename: belimo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.belimo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 09:03:39 2026 GMT\n  hsts: null\ndomains:\n- domain: belimo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/belimo/security/belimo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- HVAC
- Actuators
- Switzerland
- Manufacturing
- IoT
---
