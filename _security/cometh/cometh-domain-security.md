---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: cometh.io
  note: DNSSEC is signed and SPF/DMARC exist, but the DMARC policy is p=none (monitor only, no enforcement) and NO CAA record is published, so any public CA may issue for the domain.
  spf: true
hosts:
- cert_expires: Oct 11 02:01:48 2026 GMT
  host: www.cometh.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 06:59:42 2026 GMT
  host: docs.cometh.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 22:50:11 2026 GMT
  host: api.4337.cometh.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_cn: bundler.cometh.io
  cert_expires: Sep 21 03:40:52 2026 GMT
  host: bundler.cometh.io
  hsts: null
  http_status: 404
  https: true
  note: Kong gateway; unmatched paths return {"message":"no Route matched with those values"}.
  tls_version: TLSv1.3
- cert_cn: paymaster.cometh.io
  cert_expires: Sep 20 03:40:14 2026 GMT
  host: paymaster.cometh.io
  hsts: null
  http_status: 401
  https: true
  note: Kong key-auth; every path returns {"message":"No API key found in request"} until an apikey is supplied.
  tls_version: TLSv1.3
- cert_expires: Oct 14 18:53:03 2026 GMT
  host: status.cometh.io
  hsts: true
  hsts_max_age: 63113904
  hsts_preload: true
  http_status: 200
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 14:58:35 2026 GMT
  host: security.cometh.io
  hsts: true
  hsts_max_age: 31536000
  http_status: 200
  https: true
  note: Vanta-hosted trust centre.
  tls_version: TLSv1.3
- cert_expires: Oct 11 07:51:44 2026 GMT
  host: app.cometh.io
  hsts: null
  http_status: 200
  https: true
  note: Project dashboard where apikey/apisecret are issued; serves no HSTS header.
  tls_version: TLSv1.3
- cert_issuer: C=US, ST=California, L=San Francisco, O=Kong, OU=IT Department, CN=localhost
  cert_subject: C=US, ST=California, L=San Francisco, O=Kong, OU=IT Department, CN=localhost
  cert_valid: 2026-08-16 to 2046-08-11
  host: api.marketplace.cometh.io
  hsts: null
  https: false
  note: HOST IS BROKEN FOR TLS. The name resolves (CNAME entrypoint.core.cometh.tech) but the gateway answers with Kong's DEFAULT self-signed localhost certificate, so no client can verify it; with verification disabled the gateway returns 404 "no Route matched with those values". The still-published @cometh/marketplace-sdk targets this host — see lifecycle/cometh-lifecycle.yml.
  tls_error: 'CERTIFICATE_VERIFY_FAILED: self-signed certificate'
  tls_version: null
- cert_subject: O=Kong, CN=localhost (default certificate)
  host: api.checkout.cometh.io
  hsts: null
  https: false
  note: Same failure mode as api.marketplace.cometh.io; targeted by the still-published @cometh/checkout-sdk.
  tls_error: 'CERTIFICATE_VERIFY_FAILED: self-signed certificate'
  tls_version: null
kind: domain-security
layout: security
method: probed
name: Cometh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cometh, probed live across 10 host(s) and 1 registrable domain(s). 8 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Cometh
provider_slug: cometh
slug: cometh-domain-security
source_filename: cometh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cometh.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 02:01:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.cometh.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 06:59:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.4337.cometh.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 22:50:11 2026 GMT\n  hsts: null\n- host: bundler.cometh.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 03:40:52 2026 GMT\n  cert_cn: bundler.cometh.io\n  hsts: null\n  http_status: 404\n  note: 'Kong gateway; unmatched paths return {\"message\":\"no Route matched with those values\"}.'\n- host: paymaster.cometh.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 03:40:14 2026 GMT\n  cert_cn: paymaster.cometh.io\n  hsts: null\n  http_status: 401\n  note: 'Kong key-auth;\
  \ every path returns {\"message\":\"No API key found in request\"} until an apikey is supplied.'\n- host: status.cometh.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 18:53:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63113904\n  hsts_preload: true\n  http_status: 200\n- host: security.cometh.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 14:58:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  http_status: 200\n  note: Vanta-hosted trust centre.\n- host: app.cometh.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 07:51:44 2026 GMT\n  hsts: null\n  http_status: 200\n  note: Project dashboard where apikey/apisecret are issued; serves no HSTS header.\n- host: api.marketplace.cometh.io\n  https: false\n  tls_version: null\n  tls_error: 'CERTIFICATE_VERIFY_FAILED: self-signed certificate'\n  cert_subject: 'C=US, ST=California, L=San Francisco, O=Kong, OU=IT Department, CN=localhost'\n  cert_issuer: 'C=US, ST=California, L=San Francisco,\
  \ O=Kong, OU=IT Department, CN=localhost'\n  cert_valid: 2026-08-16 to 2046-08-11\n  hsts: null\n  note: >-\n    HOST IS BROKEN FOR TLS. The name resolves (CNAME entrypoint.core.cometh.tech) but the gateway answers with Kong's\n    DEFAULT self-signed localhost certificate, so no client can verify it; with verification disabled the gateway\n    returns 404 \"no Route matched with those values\". The still-published @cometh/marketplace-sdk targets this host —\n    see lifecycle/cometh-lifecycle.yml.\n- host: api.checkout.cometh.io\n  https: false\n  tls_version: null\n  tls_error: 'CERTIFICATE_VERIFY_FAILED: self-signed certificate'\n  cert_subject: 'O=Kong, CN=localhost (default certificate)'\n  hsts: null\n  note: Same failure mode as api.marketplace.cometh.io; targeted by the still-published @cometh/checkout-sdk.\ndomains:\n- domain: cometh.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  note: >-\n    DNSSEC is signed and SPF/DMARC exist, but the DMARC\
  \ policy is p=none (monitor only, no enforcement) and NO CAA\n    record is published, so any public CA may issue for the domain.\nx-findings:\n- 'Two API hostnames (api.marketplace, api.checkout) present Kong''s default self-signed localhost certificate — unusable over TLS.'\n- 'No CAA record on cometh.io; DMARC is p=none.'\n- 'No HSTS on the three live API hosts (api.4337, bundler, paymaster) nor on the app.cometh.io dashboard.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cometh/refs/heads/main/security/cometh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Blockchain
- account-abstraction
- erc-4337
- smart-wallet
- paymaster
- bundler
- passkeys
- webauthn
- gasless-transactions
- DeFi
- custody
- staking
- Payments
- json-rpc
- mica
- safe
- Web3
---
