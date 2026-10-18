---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cci-online.org
  spf: true
hosts:
- cert_expires: Nov 20 00:30:54 2026 GMT
  host: cci-online.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cci Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CCI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CCI
provider_slug: cci
slug: cci-domain-security
source_filename: cci-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cci-online.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 00:30:54 2026 GMT\n  hsts: false\ndomains:\n- domain: cci-online.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cci/refs/heads/main/security/cci-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- Credentialing
- Certification
- Non-Profit
- Cardiovascular
---
