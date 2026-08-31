---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1;p=quarantine;rua=mailto:dmarc@ianacare.com;pct=100;adkim=r;aspf=r
  dnssec: false
  domain: ianacare.com
  note: SPF includes Paubox, a HIPAA-compliant email relay — consistent with the HIPAA posture stated in the privacy policy. No CAA records and no DNSSEC.
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:mail.zendesk.com include:amazonses.com include:_spf.paubox.com ~all
hosts:
- cert_expires: Sep 25 10:08:26 2026 GMT
  host: ianacare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 00:10:43 2026 GMT
  host: auth.ianacare.com
  hsts: true
  hsts_header: max-age=31536000; includeSubDomains
  https: true
  note: Auth0 custom domain (CNAME prod-env-ianacare-cd-wcczcfxw9amotowp.edge.tenants.us.auth0.com).
  tls_version: TLSv1.3
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: api.ianacare.com
  hsts: false
  https: true
  note: CloudFront (d3k3w0z7cvvteo.cloudfront.net); HTTP 403 on every path.
  tls_version: TLSv1.3
- cert_expires: Nov 13 12:56:59 2026 GMT
  host: iana.ianacare.com
  hsts: false
  https: true
  note: Bearer-token API host; HTTP 401 auth_denied on /api and /api/v1.
  tls_version: TLSv1.3
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: app.ianacare.com
  hsts: false
  https: true
  note: SPA web client.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ianacare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ianacare, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ianacare
provider_slug: ianacare
slug: ianacare-domain-security
source_filename: ianacare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every ianacare host found via certificate transparency\nnote: >-\n  Host list widened beyond apis.yml by enumerating ianacare.com subdomains through\n  api.certspotter.com on 2026-08-22. HSTS is present only on the Auth0-backed identity\n  host; the marketing site, the CloudFront API edge, the bearer-token API host and the\n  web app all answer without a Strict-Transport-Security header.\nhosts:\n- host: ianacare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 10:08:26 2026 GMT\n  hsts: false\n- host: auth.ianacare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 00:10:43 2026 GMT\n  hsts: true\n  hsts_header: max-age=31536000; includeSubDomains\n  note: Auth0 custom domain (CNAME prod-env-ianacare-cd-wcczcfxw9amotowp.edge.tenants.us.auth0.com).\n- host: api.ianacare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: false\n\
  \  note: CloudFront (d3k3w0z7cvvteo.cloudfront.net); HTTP 403 on every path.\n- host: iana.ianacare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 12:56:59 2026 GMT\n  hsts: false\n  note: Bearer-token API host; HTTP 401 auth_denied on /api and /api/v1.\n- host: app.ianacare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: false\n  note: SPA web client.\ndomains:\n- domain: ianacare.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:mail.zendesk.com include:amazonses.com include:_spf.paubox.com ~all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_record: v=DMARC1;p=quarantine;rua=mailto:dmarc@ianacare.com;pct=100;adkim=r;aspf=r\n  note: >-\n    SPF includes Paubox, a HIPAA-compliant email relay — consistent with the HIPAA\n    posture stated in the privacy policy. No CAA records and no DNSSEC.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ianacare/refs/heads/main/security/ianacare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Caregiving
- Employee Benefits
- Digital Health
- Care Navigation
- Health Plans
- Mobile Application
- Identity
---
