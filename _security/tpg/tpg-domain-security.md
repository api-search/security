---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tpg.com
  spf: true
hosts:
- cert_expires: Aug 29 20:42:04 2026 GMT
  host: www.tpg.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.tpg.com
  https: false
- host: api.tpg.com
  https: false
kind: domain-security
layout: security
method: probed
name: Tpg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TPG Inc, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TPG Inc
provider_slug: tpg
slug: tpg-domain-security
source_filename: tpg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tpg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 20:42:04 2026 GMT\n  hsts: false\n- host: developer.tpg.com\n  https: false\n- host: api.tpg.com\n  https: false\ndomains:\n- domain: tpg.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tpg/refs/heads/main/security/tpg-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Private Equity
- Alternative Assets
- Investment
---
