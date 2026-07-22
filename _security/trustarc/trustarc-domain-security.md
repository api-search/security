---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trustarc.com
  spf: true
hosts:
- cert_expires: Aug 18 11:13:40 2026 GMT
  host: trustarc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trustarc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TrustArc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TrustArc
provider_slug: trustarc
slug: trustarc-domain-security
source_filename: trustarc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trustarc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 11:13:40 2026 GMT\n  hsts: false\ndomains:\n- domain: trustarc.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trustarc/refs/heads/main/security/trustarc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Privacy
- Data Privacy
- Privacy Management
- Consent Management
- Cookie Consent
- Preference Management
- Data Subject Rights
- DSR
- Privacy Governance
- Data Mapping
- Privacy Assessments
- PIA
- DPIA
- GDPR
- CCPA
- CPRA
- Data Privacy Framework
- TRUSTe
- AI Governance
- Responsible AI
- Compliance
- Certifications
- RegTech
- Trust Center
- Enterprise SaaS
---
