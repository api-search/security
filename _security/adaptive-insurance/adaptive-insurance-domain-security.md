---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adaptiveinsurance.com
  spf: true
hosts:
- cert_expires: Nov 28 23:21:28 2026 GMT
  host: www.adaptiveinsurance.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 00:28:41 2026 GMT
  host: auth.adaptiveinsurance.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: Auth0 custom-domain identity tenant; serves the OIDC and RFC 8414 discovery documents
  tls_version: TLSv1.3
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: api.adaptiveinsurance.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: Application backend. Sends helmet-style hardening headers (CSP default-src 'self', COOP/CORP same-origin, X-Content-Type-Options nosniff, X-Frame-Options SAMEORIGIN). Negotiated TLS 1.2 only on probe.
  tls_version: TLSv1.2
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: app.adaptiveinsurance.com
  hsts: false
  https: true
  note: Agent and broker portal single-page app; no Strict-Transport-Security header observed
  tls_version: TLSv1.2
hosts_probed: 4
kind: domain-security
layout: security
method: probed
name: Adaptive Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adaptive Insurance, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Adaptive Insurance
provider_slug: adaptive-insurance
slug: adaptive-insurance-domain-security
source_filename: adaptive-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: >-\n  live DNS/TLS/HTTP probes of apis.yml hosts (probe-domain-security.py), extended by hand\n  with the identity, portal and application-backend hosts found during contract discovery\nhosts:\n- host: www.adaptiveinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:21:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: auth.adaptiveinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 00:28:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: Auth0 custom-domain identity tenant; serves the OIDC and RFC 8414 discovery documents\n- host: api.adaptiveinsurance.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: >-\n    Application backend. Sends helmet-style hardening headers (CSP default-src 'self',\n    COOP/CORP same-origin, X-Content-Type-Options nosniff, X-Frame-Options SAMEORIGIN).\n\
  \    Negotiated TLS 1.2 only on probe.\n- host: app.adaptiveinsurance.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: false\n  note: Agent and broker portal single-page app; no Strict-Transport-Security header observed\ndomains:\n- domain: adaptiveinsurance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adaptive-insurance/refs/heads/main/security/adaptive-insurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Insurtech
- Parametric Insurance
- Specialty Insurance
- Climate Risk
- Weather Data
- Managing General Agent
- Flood
- Power Outage
---
