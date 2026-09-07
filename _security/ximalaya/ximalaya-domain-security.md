---
description: ''
domains:
- caa:
  - waf.c.ximalaya.com.
  dmarc: false
  dnssec: true
  domain: ximalaya.com
  spf: true
hosts:
- cert_expires: Feb 20 09:56:09 2027 GMT
  host: www.ximalaya.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 20 09:56:09 2027 GMT
  host: open.ximalaya.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- host: api.ximalaya.com
  hsts: false
  https: true
  note: 'The automated probe first recorded https:false, which was a false negative — an openssl s_client handshake to this host hangs rather than completing. Corrected 2026-09-04 after a direct HTTPS request succeeded: GET https://api.ximalaya.com/oauth2/v2/access_token returned HTTP 400 with a valid certificate (curl ssl_verify_result=0) and the documented JSON error envelope. TLS protocol version could not be negotiated by the probe and is therefore not recorded rather than guessed.'
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Ximalaya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ximalaya, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Ximalaya
provider_slug: ximalaya
slug: ximalaya-domain-security
source_filename: ximalaya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ximalaya.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 20 09:56:09 2027 GMT\n  hsts: false\n- host: open.ximalaya.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 20 09:56:09 2027 GMT\n  hsts: false\n- host: api.ximalaya.com\n  https: true\n  hsts: false\n  note: >-\n    The automated probe first recorded https:false, which was a false negative — an\n    openssl s_client handshake to this host hangs rather than completing. Corrected\n    2026-09-04 after a direct HTTPS request succeeded: GET\n    https://api.ximalaya.com/oauth2/v2/access_token returned HTTP 400 with a valid\n    certificate (curl ssl_verify_result=0) and the documented JSON error envelope.\n    TLS protocol version could not be negotiated by the probe and is therefore not\n    recorded rather than guessed.\ndomains:\n- domain: ximalaya.com\n  dnssec: true\n\
  \  caa:\n  - waf.c.ximalaya.com.\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ximalaya/refs/heads/main/security/ximalaya-domain-security.yml
summary_line: TLSv1.2 · DNSSEC
tags:
- Company
- Audio
- Podcasts
- Audiobooks
- Media
- Content Distribution
- Streaming
- China
- Entertainment
---
