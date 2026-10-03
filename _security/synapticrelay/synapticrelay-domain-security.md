---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: synapticrelay.com
  spf: false
hosts:
- cert_expires: Dec 13 17:04:05 2026 GMT
  host: synapticrelay.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Synapticrelay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SynapticRelay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: SynapticRelay
provider_slug: synapticrelay
slug: synapticrelay-domain-security
source_filename: synapticrelay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: synapticrelay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 17:04:05 2026 GMT\n  hsts: false\ndomains:\n- domain: synapticrelay.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synapticrelay/refs/heads/main/security/synapticrelay-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Freelance
- Artificial Intelligence
- Multilingual
- NoCommission
---
