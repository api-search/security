---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: destatis.de
  spf: true
hosts:
- cert_expires: Oct 20 05:20:23 2026 GMT
  host: www.destatis.de
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Genesis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GENESIS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GENESIS
provider_slug: genesis
slug: genesis-domain-security
source_filename: genesis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.destatis.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 05:20:23 2026 GMT\n  hsts: false\ndomains:\n- domain: destatis.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genesis/refs/heads/main/security/genesis-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Open Data
- Public APIs
---
