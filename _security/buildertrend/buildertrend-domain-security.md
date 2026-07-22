---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 0 iodef "mailto:domain@buildertrend.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: buildertrend.com
  spf: true
hosts:
- cert_expires: Sep 20 07:51:26 2026 GMT
  host: buildertrend.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Buildertrend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buildertrend, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Buildertrend
provider_slug: buildertrend
slug: buildertrend-domain-security
source_filename: buildertrend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buildertrend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 07:51:26 2026 GMT\n  hsts: null\ndomains:\n- domain: buildertrend.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:domain@buildertrend.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buildertrend/refs/heads/main/security/buildertrend-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Construction
- Construction Management
- Residential Construction
- Home Builders
- Remodeling
- Specialty Contractors
- Project Management
- Job Costing
- Estimating
- Scheduling
- CRM
- Proposals
- Change Orders
- Purchase Orders
- Invoicing
- Client Portal
- Subcontractor Portal
- Mobile Apps
- SaaS
- Vertical SaaS
---
