---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: 6sense.com
  spf: true
hosts:
- cert_expires: Sep 13 19:06:08 2026 GMT
  host: 6sense.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 6Sense Insights Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 6Sense Insights, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: 6Sense Insights
provider_slug: 6sense-insights
slug: 6sense-insights-domain-security
source_filename: 6sense-insights-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 6sense.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 19:06:08 2026 GMT\n  hsts: null\ndomains:\n- domain: 6sense.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/6sense-insights/refs/heads/main/security/6sense-insights-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- ABM
- Account-Based Marketing
- Intent Data
- B2B
- Predictive Analytics
- Revenue
- Sales Intelligence
- Marketing Technology
- AI
- Data Enrichment
---
