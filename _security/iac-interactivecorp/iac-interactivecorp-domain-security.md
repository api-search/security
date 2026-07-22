---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: iac.com
  spf: true
hosts:
- cert_expires: Sep  1 15:03:00 2026 GMT
  host: www.iac.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iac Interactivecorp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IAC/InterActiveCorp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: IAC/InterActiveCorp
provider_slug: iac-interactivecorp
slug: iac-interactivecorp-domain-security
source_filename: iac-interactivecorp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iac.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 15:03:00 2026 GMT\n  hsts: null\ndomains:\n- domain: iac.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iac-interactivecorp/refs/heads/main/security/iac-interactivecorp-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Conglomerate
- Internet
- Media
- Parent Company
---
