---
description: ''
domains:
- caa:
  - 0 issuewild "auth0.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazonaws.com"
  - 0 issue "auth0.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: careporthealth.com
  spf: true
hosts:
- cert_expires: Aug 20 01:24:39 2026 GMT
  host: careporthealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Careport Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Careport Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Careport Health
provider_slug: careport-health
slug: careport-health-domain-security
source_filename: careport-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: careporthealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 01:24:39 2026 GMT\n  hsts: false\ndomains:\n- domain: careporthealth.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"auth0.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"auth0.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/careport-health/refs/heads/main/security/careport-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Care Coordination
- Discharge Planning
- Post-Acute Care
- Transitional Care
- Health IT
- Interoperability
- Value-Based Care
- Referral Management
- Utilization Management
---
