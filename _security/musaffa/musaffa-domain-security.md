---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: musaffa.com
  spf: true
hosts:
- cert_expires: Oct 16 06:06:35 2026 GMT
  host: musaffa.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 17:42:31 2026 GMT
  host: api.musaffa.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- host: platform.musaffa.com
  https: false
  probe_note: Recorded as https:false because neither `openssl s_client` nor curl could complete a clean TLS session with this host on 2026-08-26 (curl reported HTTP status 000, no certificate could be read). The host DOES serve content over https — a 938KB Next.js SPA shell came back for every path tried — but the connection terminates abnormally, so no TLS version, certificate expiry or HSTS value could be measured. Treat this as an unmeasured host, not as a plaintext one.
kind: domain-security
layout: security
method: probed
name: Musaffa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Musaffa, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Musaffa
provider_slug: musaffa
slug: musaffa-domain-security
source_filename: musaffa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: musaffa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 06:06:35 2026 GMT\n  hsts: false\n- host: api.musaffa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 17:42:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: platform.musaffa.com\n  https: false\n  probe_note: >-\n    Recorded as https:false because neither `openssl s_client` nor curl could complete a clean TLS\n    session with this host on 2026-08-26 (curl reported HTTP status 000, no certificate could be\n    read). The host DOES serve content over https — a 938KB Next.js SPA shell came back for every\n    path tried — but the connection terminates abnormally, so no TLS version, certificate expiry or\n    HSTS value could be measured. Treat this as an unmeasured host, not as a plaintext one.\ndomains:\n- domain: musaffa.com\n  dnssec: false\n  caa: []\n\
  \  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/musaffa/refs/heads/main/security/musaffa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Islamic Finance
- Shariah Compliance
- Halal Investing
- Stock Screening
- Financial Data
- ETFs
- Market Data
- Fintech
- Investing
- Compliance
- Zakat
- Company
---
