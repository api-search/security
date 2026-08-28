---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: microconnect.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: mcisaas.com
  spf: false
hosts:
- cert_expires: Oct  6 06:08:59 2026 GMT
  host: www.microconnect.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 10 01:48:24 2026 GMT
  host: open.microconnect.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: api.mcisaas.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expired: true
  cert_expires: Nov 27 23:59:59 2024 GMT
  cert_issuer: GeoTrust CN RSA CA G1
  cert_subject: C=CN, ST=海南省, L=海口市, O=滴灌通管理咨询（海南）有限公司, CN=microconnect.cn
  host: open.microconnect.cn
  https: true
  note: EXPIRED CERTIFICATE. open.microconnect.com (valid cert) 301-redirects here, so the Open Platform is unreachable to any TLS-verifying client. Observed 2026-08-25.
  tls_version: TLSv1.2
- cert_expired: false
  cert_expires: Jan 10 23:59:59 2027 GMT
  cert_subject: C=CN, ST=海南省, L=海口市, O=滴灌通管理咨询（海南）有限公司, CN=*.mcisaas.com
  host: kc.mcisaas.com
  https: true
  note: Keycloak identity provider. Certificate organisation confirms first-party ownership of the mcisaas.com estate.
  tls_version: TLSv1.2
- cert_expired: false
  cert_expires: Dec  2 06:07:11 2026 GMT
  cert_subject: CN=*.mcex.mo
  host: mcex.mo
  https: true
  tls_version: TLSv1.3
- cert_expired: false
  cert_expires: Oct  6 06:08:59 2026 GMT
  cert_subject: CN=*.microconnect.com
  host: mt.microconnect.com
  https: true
  note: M-Terminal investor terminal.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Micro Connect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Micro Connect, probed live across 7 host(s) and 2 registrable domain(s). 7 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Micro Connect
provider_slug: micro-connect
slug: micro-connect-domain-security
source_filename: micro-connect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.microconnect.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  6 06:08:59 2026 GMT\n  hsts: false\n- host: open.microconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 01:48:24 2026 GMT\n  hsts: null\n- host: api.mcisaas.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: open.microconnect.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_subject: C=CN, ST=海南省, L=海口市, O=滴灌通管理咨询（海南）有限公司, CN=microconnect.cn\n  cert_issuer: GeoTrust CN RSA CA G1\n  cert_expires: Nov 27 23:59:59 2024 GMT\n  cert_expired: true\n  note: EXPIRED CERTIFICATE. open.microconnect.com (valid cert) 301-redirects here, so the Open Platform\n    is unreachable to any TLS-verifying client. Observed 2026-08-25.\n- host: kc.mcisaas.com\n  https: true\n  tls_version: TLSv1.2\n\
  \  cert_subject: C=CN, ST=海南省, L=海口市, O=滴灌通管理咨询（海南）有限公司, CN=*.mcisaas.com\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  cert_expired: false\n  note: Keycloak identity provider. Certificate organisation confirms first-party ownership of the mcisaas.com\n    estate.\n- host: mcex.mo\n  https: true\n  tls_version: TLSv1.3\n  cert_subject: CN=*.mcex.mo\n  cert_expires: Dec  2 06:07:11 2026 GMT\n  cert_expired: false\n- host: mt.microconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_subject: CN=*.microconnect.com\n  cert_expires: Oct  6 06:08:59 2026 GMT\n  cert_expired: false\n  note: M-Terminal investor terminal.\ndomains:\n- domain: microconnect.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: mcisaas.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\nnote: 'Probe extended by hand on 2026-08-25 to cover hosts the automated probe does not read out of apis.yml:\n  the Open Platform origin behind the open.microconnect.com\
  \ redirect, the Keycloak identity provider,\n  the MCEX exchange host and the M-Terminal host. KEY FINDING: open.microconnect.cn serves a certificate\n  that expired 2024-11-27.'\nownership_evidence: TLS certificates on api.mcisaas.com, kc.mcisaas.com and open.microconnect.cn are all\n  issued to O=滴灌通管理咨询（海南）有限公司 (Micro Connect Management Consulting (Hainan) Co., Ltd), confirming the\n  mcisaas.com estate is first-party Micro Connect infrastructure and not a third-party vendor domain.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/micro-connect/refs/heads/main/security/micro-connect-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Financial Services
- Capital Markets
- Exchanges
- Revenue Based Financing
- Fintech
- Investing
- Small Business
- Hong Kong
- Macao
- China
---
