---
api_specs:
- filename: whisperr-inc-runtime-openapi.json
  format: json
  label: Whisperr Runtime API
  slug: whisperr-runtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whisperr-inc/refs/heads/main/openapi/whisperr-inc-runtime-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: whisperr.net
  spf: false
  verification:
    caa: No CAA records (three consecutive empty responses from 1.1.1.1).
    dmarc: No TXT record at _dmarc.whisperr.net.
    impact: Material for this provider specifically — Whisperr sends retention email on its customers' behalf via a provisioned delivery server, so the absence of SPF and DMARC on its own domain is worth the provider's attention.
    note: The automated probe first returned a resolver timeout string in the caa field; that was a transient DNS failure, not a record. Re-queried directly against 1.1.1.1 on 2026-08-13 and confirmed by hand.
    spf: No v=spf1 record. The only TXT records on the apex are ownership verifications (MS=, google-site-verification=).
hosts:
- cert_expires: Oct 11 19:24:56 2026 GMT
  host: whisperr.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 09:06:27 2026 GMT
  host: docs.whisperr.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 17:09:55 2026 GMT
  host: api.whisperr.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Whisperr Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Whisperr, Inc., probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Whisperr, Inc.
provider_slug: whisperr-inc
slug: whisperr-inc-domain-security
source_filename: whisperr-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: whisperr.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 19:24:56 2026 GMT\n  hsts: false\n- host: docs.whisperr.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 09:06:27 2026 GMT\n  hsts: false\n- host: api.whisperr.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 17:09:55 2026 GMT\n  hsts: null\ndomains:\n- domain: whisperr.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  verification:\n    note: >-\n      The automated probe first returned a resolver timeout string in the caa\n      field; that was a transient DNS failure, not a record. Re-queried directly\n      against 1.1.1.1 on 2026-08-13 and confirmed by hand.\n    caa: No CAA records (three consecutive empty responses from 1.1.1.1).\n    spf: >-\n      No v=spf1 record. The only TXT records on the apex are ownership\n      verifications\
  \ (MS=, google-site-verification=).\n    dmarc: No TXT record at _dmarc.whisperr.net.\n    impact: >-\n      Material for this provider specifically — Whisperr sends retention email on\n      its customers' behalf via a provisioned delivery server, so the absence of\n      SPF and DMARC on its own domain is worth the provider's attention.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whisperr-inc/refs/heads/main/security/whisperr-inc-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Customer Retention
- Churn
- Marketing Automation
- Artificial Intelligence
- Software-as-a-Service
- Subscription
- Customer Engagement
- Event Ingestion
- Analytics
- Customer Data
- Email Delivery
- Agents
---
