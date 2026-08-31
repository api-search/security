---
api_specs:
- filename: fudan-identity-openapi.yml
  format: yaml
  label: Fudan University Unified Identity — OpenID Connect
  slug: identity-oidc
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fudan/refs/heads/main/openapi/fudan-identity-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fudan.edu.cn
  spf: true
hosts:
- cert_expires: Apr 10 23:59:59 2027 GMT
  host: www.fudan.edu.cn
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr 10 23:59:59 2027 GMT
  host: dvn.fudan.edu.cn
  hsts: false
  https: true
  note: Now serves only a meta-refresh redirect to https://rdr.fudan.edu.cn/datahome/ (probed 2026-08-30).
  tls_version: TLSv1.3
- cert_expires: Apr 10 23:59:59 2027 GMT
  host: id.fudan.edu.cn
  hsts: false
  https: true
  note: OpenID Connect provider. Discovery document and JWKS served without authentication.
  tls_version: TLSv1.2+
- cert_expires: Apr 10 23:59:59 2027 GMT
  host: idpfudan.fudan.edu.cn
  hsts: false
  https: true
  note: Shibboleth SAML 2.0 identity provider registered in CARSI/eduGAIN. SOAP attribute query on port 8443.
  tls_version: TLSv1.2
- cert_expires: Apr 10 23:59:59 2027 GMT
  host: rdr.fudan.edu.cn
  hsts: false
  https: true
  note: Research data platform. Replaced dvn.fudan.edu.cn.
  tls_version: TLSv1.2+
kind: domain-security
layout: security
method: probed
name: Fudan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fudan University, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fudan University
provider_slug: fudan
slug: fudan-domain-security
source_filename: fudan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "x-method: derived\ngenerated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fudan.edu.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 10 23:59:59 2027 GMT\n  hsts: null\n- host: dvn.fudan.edu.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 10 23:59:59 2027 GMT\n  hsts: false\n  note: Now serves only a meta-refresh redirect to https://rdr.fudan.edu.cn/datahome/ (probed 2026-08-30).\n- host: id.fudan.edu.cn\n  https: true\n  tls_version: TLSv1.2+\n  cert_expires: Apr 10 23:59:59 2027 GMT\n  hsts: false\n  note: OpenID Connect provider. Discovery document and JWKS served without authentication.\n- host: idpfudan.fudan.edu.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr 10 23:59:59 2027 GMT\n  hsts: false\n  note: Shibboleth SAML 2.0 identity provider registered in CARSI/eduGAIN. SOAP attribute query on port\n    8443.\n- host: rdr.fudan.edu.cn\n  https: true\n  tls_version:\
  \ TLSv1.2+\n  cert_expires: Apr 10 23:59:59 2027 GMT\n  hsts: false\n  note: Research data platform. Replaced dvn.fudan.edu.cn.\ndomains:\n- domain: fudan.edu.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nmodified: '2026-08-30'\nnote: Hosts added 2026-08-30 by the university pipeline after the identity and research-data surfaces\n  were probed. dvn.fudan.edu.cn is retained because it still resolves, but it now only meta-refreshes\n  to rdr.fudan.edu.cn.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fudan/refs/heads/main/security/fudan-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- University
- Higher Education
- Education
- China
- Shanghai
- C9 League
- Identity Federation
- Research Data
- Single Sign-On
---
