---
description: 'Transport and DNS security posture for NTT DOCOMO, Inc.''s public hosts. The headline finding is a split: the corporate host and the OIDC issuer negotiate TLS 1.3, but id.smt.docomo.ne.jp — the d ACCOUNT authorization endpoint host, where roughly 90 million users authenticate — caps at TLS 1.2, serves no HSTS, and rejects RFC 5746 secure renegotiation. Neither docomo.ne.jp nor nttdocomo.co.jp is DNSSEC-signed or publishes a CAA record.'
domains:
- caa: []
  dmarc: true
  dmarc_pct: 100
  dmarc_policy: quarantine
  dmarc_rua: mailto:docomo00001-ra@dmarc25.jp
  dmarc_subdomain_policy: reject
  dnssec: false
  domain: docomo.ne.jp
  spf: true
  spf_policy: ~all
  spf_record: v=spf1 +ip4:203.138.203.0/24 +ip4:210.153.87.192/29 +ip4:210.153.87.224/29 +ip4:202.212.37.97 +ip4:202.212.37.98 +ip4:202.212.37.100 +ip4:202.212.37.113 +ip4:202.212.37.103 +ip4:202.212.37.104 +ip4:1.73.231.0/26 +ip4:1.75.151.128/25 +ip4:1.75.146.128/25 +ip4:49.102.168.0/21 ~all
- caa: []
  dmarc: true
  dmarc_pct: 100
  dmarc_policy: none
  dmarc_rua: mailto:dm0mlsugqaev8.rua@dp.smtps.jp
  dmarc_subdomain_policy: none
  dnssec: false
  domain: nttdocomo.co.jp
  notes: The corporate domain runs DMARC in monitor mode (p=none) while the consumer/service domain enforces quarantine with sp=reject.
  spf: true
  spf_policy: ~all
hosts:
- cert_expires: Oct 19 04:19:21 2026 GMT
  cert_issuer: GlobalSign nv-sa
  host: www.docomo.ne.jp
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 15768000
  hsts_preload: false
  http_version: HTTP/2
  https: true
  role: Corporate site and surviving public developer information page
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:59:59 2026 GMT
  cert_issuer: DigiCert Inc
  host: conf.uw.docomo.ne.jp
  hsts: false
  http_version: HTTP/2
  https: true
  notes: Fronted by CloudFront over an AWS API Gateway origin (server openresty, apigw-requestid and x-amz-cf-id response headers). Returns 403 to every path except /.well-known/openid-configuration.
  role: d ACCOUNT Connect OpenID Provider (issuer, token, userinfo)
  tls_version: TLSv1.3
- cert_expires: Sep 30 14:59:59 2026 GMT
  cert_issuer: GlobalSign nv-sa (GlobalSign RSA OV SSL CA 2018)
  cert_subject: C=JP, ST=Tokyo, L=Chiyoda-Ku, O=NTT DOCOMO.INC, CN=id.smt.docomo.ne.jp
  host: id.smt.docomo.ne.jp
  hsts: false
  http_version: HTTP/1.1
  https: true
  notes: TLS 1.3 handshake fails (curl --tlsv1.3 --tls-max 1.3 returns no response); TLS 1.2 succeeds and serves HTTP 200. The server does not advertise the RFC 5746 renegotiation_info extension, so a default OpenSSL 3 client refuses the connection with UNSAFE_LEGACY_RENEGOTIATION_DISABLED. This is the host that carries the OIDC authorization endpoint /cgi8/oidc/authorize.
  role: d ACCOUNT authorization endpoint and business documentation host
  secure_renegotiation: false
  tls13_supported: false
  tls_version: TLSv1.2
- cert_expires: Sep 30 14:59:59 2026 GMT
  cert_issuer: GlobalSign nv-sa
  host: fr-end.oidc.if.cilite.docomo.ne.jp
  hsts: false
  http_version: HTTP/2
  https: true
  role: JWKS host for d ACCOUNT Connect
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ntt Docomo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NTT Docomo, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: NTT Docomo
provider_slug: ntt-docomo
slug: ntt-docomo-domain-security
source_filename: ntt-docomo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: >-\n  Live TLS handshakes, HTTP HEAD and dig queries against every host in apis.yml\n  plus the JWKS host advertised by the d ACCOUNT Connect discovery document.\n  Probed 2026-07-25. The registrable domain was corrected by hand to\n  docomo.ne.jp — ne.jp is a Japanese second-level generic, not a registrable\n  domain, and the automated pass had queried it. id.smt.docomo.ne.jp was also\n  re-probed by hand: the automated pass recorded https:false because its\n  handshake fails under a default OpenSSL 3 context (see below), not because\n  the host lacks HTTPS.\ndescription: >-\n  Transport and DNS security posture for NTT DOCOMO, Inc.'s public hosts. The\n  headline finding is a split: the corporate host and the OIDC issuer negotiate\n  TLS 1.3, but id.smt.docomo.ne.jp — the d ACCOUNT authorization endpoint host,\n  where roughly 90 million users authenticate — caps at TLS 1.2, serves no HSTS,\n  and rejects RFC 5746 secure renegotiation.\
  \ Neither docomo.ne.jp nor\n  nttdocomo.co.jp is DNSSEC-signed or publishes a CAA record.\nhosts:\n- host: www.docomo.ne.jp\n  role: Corporate site and surviving public developer information page\n  https: true\n  tls_version: TLSv1.3\n  http_version: HTTP/2\n  cert_issuer: GlobalSign nv-sa\n  cert_expires: Oct 19 04:19:21 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n  hsts_include_subdomains: false\n  hsts_preload: false\n- host: conf.uw.docomo.ne.jp\n  role: d ACCOUNT Connect OpenID Provider (issuer, token, userinfo)\n  https: true\n  tls_version: TLSv1.3\n  http_version: HTTP/2\n  cert_issuer: DigiCert Inc\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: false\n  notes: >-\n    Fronted by CloudFront over an AWS API Gateway origin (server openresty,\n    apigw-requestid and x-amz-cf-id response headers). Returns 403 to every\n    path except /.well-known/openid-configuration.\n- host: id.smt.docomo.ne.jp\n  role: d ACCOUNT authorization endpoint and business documentation host\n\
  \  https: true\n  tls_version: TLSv1.2\n  tls13_supported: false\n  http_version: HTTP/1.1\n  cert_issuer: GlobalSign nv-sa (GlobalSign RSA OV SSL CA 2018)\n  cert_subject: C=JP, ST=Tokyo, L=Chiyoda-Ku, O=NTT DOCOMO.INC, CN=id.smt.docomo.ne.jp\n  cert_expires: Sep 30 14:59:59 2026 GMT\n  hsts: false\n  secure_renegotiation: false\n  notes: >-\n    TLS 1.3 handshake fails (curl --tlsv1.3 --tls-max 1.3 returns no response);\n    TLS 1.2 succeeds and serves HTTP 200. The server does not advertise the\n    RFC 5746 renegotiation_info extension, so a default OpenSSL 3 client\n    refuses the connection with UNSAFE_LEGACY_RENEGOTIATION_DISABLED. This is\n    the host that carries the OIDC authorization endpoint /cgi8/oidc/authorize.\n- host: fr-end.oidc.if.cilite.docomo.ne.jp\n  role: JWKS host for d ACCOUNT Connect\n  https: true\n  tls_version: TLSv1.3\n  http_version: HTTP/2\n  cert_issuer: GlobalSign nv-sa\n  cert_expires: Sep 30 14:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: docomo.ne.jp\n\
  \  dnssec: false\n  caa: []\n  spf: true\n  spf_policy: '~all'\n  spf_record: >-\n    v=spf1 +ip4:203.138.203.0/24 +ip4:210.153.87.192/29 +ip4:210.153.87.224/29\n    +ip4:202.212.37.97 +ip4:202.212.37.98 +ip4:202.212.37.100\n    +ip4:202.212.37.113 +ip4:202.212.37.103 +ip4:202.212.37.104\n    +ip4:1.73.231.0/26 +ip4:1.75.151.128/25 +ip4:1.75.146.128/25\n    +ip4:49.102.168.0/21 ~all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_subdomain_policy: reject\n  dmarc_pct: 100\n  dmarc_rua: mailto:docomo00001-ra@dmarc25.jp\n- domain: nttdocomo.co.jp\n  dnssec: false\n  caa: []\n  spf: true\n  spf_policy: '~all'\n  dmarc: true\n  dmarc_policy: none\n  dmarc_subdomain_policy: none\n  dmarc_pct: 100\n  dmarc_rua: mailto:dm0mlsugqaev8.rua@dp.smtps.jp\n  notes: >-\n    The corporate domain runs DMARC in monitor mode (p=none) while the\n    consumer/service domain enforces quarantine with sp=reject.\nfindings:\n- severity: notable\n  finding: >-\n    id.smt.docomo.ne.jp — the d ACCOUNT authorization\
  \ endpoint host — does not\n    support TLS 1.3, sends no HSTS header, and lacks RFC 5746 secure\n    renegotiation.\n- severity: notable\n  finding: >-\n    No CAA records on either registrable domain, so no certificate-authority\n    issuance restriction is published.\n- severity: notable\n  finding: No DNSSEC on docomo.ne.jp or nttdocomo.co.jp.\n- severity: informational\n  finding: >-\n    HSTS is present only on www.docomo.ne.jp, with a six-month max-age and\n    neither includeSubDomains nor preload, so it does not protect the identity\n    hosts.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ntt-docomo/refs/heads/main/security/ntt-docomo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telecommunications
- Japan
- Mobile Network Operator
- Network APIs
- CAMARA
- Open Gateway
- Aduna
- Carrier Identity
- SIM Swap
- Number Verification
- Carrier Billing
- 5G
- Partner Gated
---
