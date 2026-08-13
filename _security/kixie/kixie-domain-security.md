---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kixie.com
  spf: true
hosts:
- cert_expires: Oct 22 09:48:42 2026 GMT
  host: www.kixie.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 01:16:02 2026 GMT
  host: developer.kixie.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: apig.kixie.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kixie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kixie, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kixie
provider_slug: kixie
slug: kixie-domain-security
source_filename: kixie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kixie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 09:48:42 2026 GMT\n  hsts: false\n- host: developer.kixie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 01:16:02 2026 GMT\n  hsts: false\n- host: apig.kixie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: kixie.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n\nfindings:\n- id: no-hsts\n  severity: medium\n  applies_to:\n  - www.kixie.com\n  - developer.kixie.com\n  finding: >-\n    No Strict-Transport-Security header on the marketing site or the developer documentation host.\n    A first visit over http:// is downgradeable.\n  remedy: Send Strict-Transport-Security with a max-age of at least 31536000 and includeSubDomains.\n- id: hsts-unknown-on-gateway\n\
  \  severity: informational\n  applies_to:\n  - apig.kixie.com\n  finding: >-\n    HSTS could not be determined on the API gateway because it returns 403 to every\n    unauthenticated request, including the probe.\n- id: dmarc-p-none\n  severity: medium\n  applies_to:\n  - kixie.com\n  finding: >-\n    DMARC is published but the policy is p=none — monitoring only. Nothing is quarantined or\n    rejected, so a spoofed kixie.com sender still lands. For a vendor whose product is outbound\n    business communication and whose support flow runs on email (API-key activation, webhook\n    provisioning, and vulnerability reports all arrive by email), an unenforced DMARC policy is a\n    weaker posture than the product implies.\n  remedy: Move to p=quarantine and then p=reject once alignment reporting is clean.\n- id: no-caa\n  severity: low\n  applies_to:\n  - kixie.com\n  finding: >-\n    No CAA record, so any public CA may issue a certificate for kixie.com or its subdomains.\n  remedy: Publish\
  \ CAA records naming the issuing CA(s), with an iodef contact.\n- id: no-dnssec\n  severity: low\n  applies_to:\n  - kixie.com\n  finding: DNSSEC is not enabled; DNS answers are not origin-authenticated.\n\nstrengths:\n- TLS 1.3 negotiated on all three reachable hosts.\n- Valid, unexpired certificates on all three hosts at the 2026-08-12 probe.\n- SPF and DMARC records both present.\n\nrelated:\n  vulnerability_disclosure: security/kixie-vulnerability-disclosure.yml\n  trust_center: security/kixie-trust-center.yml\n  well_known: well-known/kixie-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kixie/refs/heads/main/security/kixie-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Sales Engagement
- Voice
- Telephony
- SMS
- Messaging
- Contact Center
- Power Dialer
- CRM
- Webhooks
- Communications
- Revenue Operations
---
