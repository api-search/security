---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: symplr.com
  spf: true
hosts:
- cert_expires: Sep 11 15:46:33 2026 GMT
  host: www.symplr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Halo Health Symplr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Halo Health (Symplr), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Halo Health (Symplr)
provider_slug: halo-health-symplr
slug: halo-health-symplr-domain-security
source_filename: halo-health-symplr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.symplr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 15:46:33 2026 GMT\n  hsts: false\ndomains:\n- domain: symplr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/halo-health-symplr/refs/heads/main/security/halo-health-symplr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Clinical Communications
- Secure Messaging
- Care Collaboration
- On-Call Scheduling
- HL7
- EHR Integration
- HIPAA
---
