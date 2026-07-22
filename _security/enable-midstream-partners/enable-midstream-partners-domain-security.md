---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: energytransfer.com
  spf: true
hosts:
- cert_expires: Oct 25 16:38:14 2026 GMT
  host: www.energytransfer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Enable Midstream Partners Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enable Midstream Partners, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Enable Midstream Partners
provider_slug: enable-midstream-partners
slug: enable-midstream-partners-domain-security
source_filename: enable-midstream-partners-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.energytransfer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 16:38:14 2026 GMT\n  hsts: null\ndomains:\n- domain: energytransfer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enable-midstream-partners/refs/heads/main/security/enable-midstream-partners-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Acquired
- Crude Oil
- Energy
- Midstream
- Natural Gas
- Pipelines
---
